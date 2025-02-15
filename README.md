# PR GIT

This repository is an AI agent that can be used to create PRs depending on code changes, removing the hassle of crafting a good PR message and capturing all the necessary points required in a PR.

## Development Rough Draft

1. Using Git Hooks
	- Trigger the script using Git hooks when code changes are pushed.
	- The hook script will be placed in `.git/hooks`.

2. Installing Required Libraries
	- Use @octokit/rest for GitHub API interactions.
	- Use simple-git for Git commands.

3. Writing the Main Script
	- Check for Code Changes: Use simple-git to determine if there are any code changes to push.
	- Create a New Branch: Create a new branch for the changes.
	- Commit the Changes: Commit the changes to the new branch.
	- Push the Changes: Push the changes to the remote repository.
	- Create a Pull Request: Use @octokit/rest to create a pull request on GitHub.

4. Implementing the PR Creation Logic
	- Use the simple-git library to handle Git commands.
	- Use the @octokit/rest library to interact with the GitHub API.
