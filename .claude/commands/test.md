Run the full Sphinx documentation build and test suite using `./run_tests.sh` (or a specific project if one is provided as an argument, e.g. `/test en_us/course_authors/`).

Identify an appropriate virtualenv and source it before running. If an appropriate virtualenv is not found, be sure to prompt the user to either select / enter an appropriate virtualenv, create a new virtualenv, or have you install the requirements globally (not advised) before running.

After the build completes:

1. Report the total Sphinx error and warning counts clearly to the user.
2. Read the `test_root/<project>/err.log` files for any project that failed to get the full warning/error detail.
3. If there are **no errors or warnings**, confirm the build is clean and ready to push.
4. If there **are** errors or warnings:
   - List each one with its file path and line number.
   - For each issue, either:
     - **Fix it automatically** if it is straightforward (e.g. title overline too short, trailing whitespace, malformed RST directives), then re-run the tests to confirm the fix works.
     - **Explain how to fix it manually** if it requires editorial judgment (e.g. broken cross-references pointing to missing content, ambiguous section structure).
   - After attempting all auto-fixes, re-run the tests and report the final result.
