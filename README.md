If you already cloned the repository and added new files into the local repository folder, the typical Git workflow is:

1. Open terminal in the repository directory
cd /path/to/your/repository
2. Check current status

This shows which files are new, modified, or deleted.

git status
3. Add files to Git staging area

Add all files:

git add .

Or add a specific file:

git add filename.txt

Or add a specific folder:

git add foldername/
4. Verify staged files
git status

You should see files listed under:

Changes to be committed:
5. Create a commit
git commit -m "Added new files"

Use a meaningful message, for example:

git commit -m "Added Terraform configuration for AWS infrastructure"
6. Check which branch you are on
git branch

or

git branch --show-current
7. Pull latest changes first (recommended)
git pull origin <branch-name>

Example:

git pull origin main

Resolve any conflicts if Git reports them.

8. Push changes
git push origin <branch-name>

Example:

git push origin main
If Git asks for authentication

Depending on your Git provider, you may need:

Personal Access Token (PAT) instead of password
SSH key authentication

For example, with GitHub, passwords are no longer accepted for Git operations over HTTPS.

Useful commands for troubleshooting

Check remote repository:

git remote -v

See commit history:

git log --oneline -5

See differences before committing:

git diff
