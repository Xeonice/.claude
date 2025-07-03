Git Workflow Automation Prompt
Please help me automate a complete git workflow with the following steps:
Workflow Requirements:

Check Staging Area: First, check if there are any staged or unstaged changes in the current repository

Use git status to inspect the current state
If there are changes, proceed with the workflow
If no changes, inform me and ask if I want to continue anyway


Switch to Main Branch: Switch to the main branch (either master or main)

Detect which main branch exists (master or main)
Switch to that branch using git checkout or git switch
Pull the latest changes with git pull origin <main-branch>


Create New Branch: Create and switch to a new feature branch

Generate a meaningful branch name based on the changes (e.g., feature/update-dependencies, fix/bug-description)
Use git checkout -b <branch-name> or git switch -c <branch-name>


Auto-generate Commit: Create an intelligent commit message and commit changes

Stage all changes with git add .
Generate a descriptive commit message based on the file changes
Follow conventional commit format if possible (e.g., feat:, fix:, docs:, etc.)
Commit with git commit -m "<generated-message>"


Push Branch: Push the new branch to remote repository

Use git push -u origin <branch-name>


Create Pull Request: If GitHub CLI (gh) is available, create a PR

Check if gh command is installed with gh --version
If available, create a PR with: gh pr create --title "<title>" --body "<description>"
Generate appropriate PR title and description based on the changes
If gh is not available, provide instructions for manual PR creation



Additional Requirements:

Handle errors gracefully and provide clear feedback
Ask for confirmation before making destructive changes
Provide status updates at each step
If any step fails, stop the process and explain the issue
Ensure the working directory is clean before switching branches

Output Format:
Please execute each step and provide:

Clear status messages for each operation
Any errors encountered and how they were resolved
Final summary of what was accomplished
Next steps or manual actions required (if any)

Execute this workflow now for the current repository.
