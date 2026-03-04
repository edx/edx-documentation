Generate a pull request description for the current branch based on the commit history and the project's PR template.

Steps:

1. Run `git log origin/master..HEAD --oneline` to list commits in this branch.
2. Run `git diff origin/master..HEAD --stat` to see which files changed.
3. Run `git diff origin/master..HEAD` to read the full diff for context on what changed.
4. Read `.github/PULL_REQUEST_TEMPLATE.md` to get the PR template structure.

Then produce a filled-in PR description using the template:

- Write a clear, concise summary of what changed and why, based on the commits and diff. Include links to relevant files or sections if helpful.
- Leave `### Date Needed` blank (the user will fill it in if needed).
- Leave the `### Reviewers` checklist items blank for the user to fill in names.
- Check the `Ran ./run_tests.sh without warnings or errors` box only if the conversation history shows tests were run and passed cleanly.
- Leave `### HTML Version` and `### Sandbox` unchecked.
- Leave `### Post-review` unchecked.

Output the result as a plain markdown code block (wrapped in triple backticks) so the user can easily copy and paste it into a GitHub PR.
