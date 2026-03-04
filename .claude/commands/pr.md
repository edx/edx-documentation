Generate and create a pull request for the current branch against `edx/edx-documentation`.

Steps:

1. Run `git log master..HEAD --oneline` to list commits in this branch.
2. Run `git diff master..HEAD --stat` to see which files changed.
3. Run `git diff master..HEAD` to read the full diff for context on what changed.
4. Read `.github/PULL_REQUEST_TEMPLATE.md` to get the PR template structure.

Generate a PR title and description:

- **Title**: A short, descriptive title (under 70 characters) based on the commits.
- **Description**: Fill in the PR template:
  - Write a clear summary of what changed and why, based on the commits and diff.
  - Leave `### Date Needed` blank.
  - Leave `### Reviewers` checklist items blank for the user to fill in.
  - Check the `Ran ./run_tests.sh without warnings or errors` box only if the conversation history shows tests passed cleanly.
  - Leave `### HTML Version`, `### Sandbox`, and `### Post-review` unchecked.

Then:

5. **Security scan**: Search the diff for potential secrets or sensitive material. Look for patterns such as:
   - API keys, tokens, or passwords (e.g. strings matching `sk-`, `ghp_`, `xox`, `Bearer`, `token`, `secret`, `password`, `api_key` — case-insensitive)
   - Private keys or certificates (e.g. `-----BEGIN`)
   - Hardcoded credentials or connection strings
   - AWS/GCP/Azure key patterns

   If anything suspicious is found, **stop and report it to the user** before proceeding. Do not create the PR.

6. Show the user the generated title and description and ask for confirmation before proceeding.
7. If confirmed, push the current branch to `origin` if it hasn't been pushed yet (run `git push -u origin HEAD`).
8. Create the PR using:
   ```
   gh pr create --repo edx/edx-documentation --base master --title "<title>" --body "<description>"
   ```
9. Output the PR URL so the user can open it.
