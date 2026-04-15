# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Status

This is an organizational fork of the upstream edx-documentation repository. While the upstream is deprecated, this fork is actively maintained to keep documentation up to date for our organization.

## Common Commands

```bash
# Install Python dependencies
make requirements

# Build all documentation projects (runs tests)
./run_tests.sh

# Build a single documentation project
./run_tests.sh en_us/developers/

# Start live-reload development server for a project
pip install -r shared/tools.txt
./develop.sh en_us/developers/ [port]   # Default port: 9090

# Update/recompile Python requirements
make upgrade

# Clean build artifacts
make clean

# Create translation files for Transifex
make i18n
```

## Architecture

This is a **Sphinx-based static documentation site** using reStructuredText (RST) source files. There is no application code — only documentation content and build configuration.

**Technology stack:**
- Markup: reStructuredText (RST)
- Build: Sphinx with `sphinx-book-theme`
- Hosting: Read the Docs (docs.edx.org)
- Translations: Transifex (only 3 projects: edx_students, open_edx_course_authors, open_edx_release_notes)
- CI: GitHub Actions (`.github/workflows/build.yml`) — builds on push to `master` and PRs

**Project layout:**

Each of the 13 documentation projects lives under `en_us/<project_name>/` with standard Sphinx structure:
```
en_us/<project>/
├── Makefile
└── source/
    ├── conf.py
    └── index.rst + content .rst files
```

**Shared configuration** in `shared/conf.py` and `shared/edxconf.py` is imported by individual project `conf.py` files.

**Build behavior:** `run_tests.sh` builds all projects in nit-picky Sphinx mode (`-n`) with 4 parallel workers. Warnings and errors are written to log files in `test_root/` via `-w`, then parsed — a build with any Sphinx warnings or errors is considered a failure.

**PR requirements:** Run `./run_tests.sh` without warnings or errors before submitting. PRs require SME, product, and partner support sign-off per `.github/PULL_REQUEST_TEMPLATE.md`.
