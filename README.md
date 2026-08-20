If you already cloned the repository and added new files into the local repository folder, the typical Git workflow is:<br/>
<br/>
1. Open terminal in the repository directory<br/>
cd /path/to/your/repository<br/>
2. Check current status<br/>
<br/>
This shows which files are new, modified, or deleted.<br/>
<br/>
git status<br/>
3. Add files to Git staging area<br/>
<br/>
Add all files:<br/>
<br/>
git add .<br/>
<br/>
Or add a specific file:<br/>
<br/>
git add filename.txt<br/>
<br/>
Or add a specific folder:<br/>
<br/>
git add foldername/<br/>
4. Verify staged files<br/>
git status<br/>
<br/>
You should see files listed under:<br/>
<br/>
Changes to be committed:<br/>
5. Create a commit<br/>
git commit -m "Added new files"<br/>
<br/>
Use a meaningful message, for example:<br/>
<br/>
git commit -m "Added Terraform configuration for AWS infrastructure"<br/>
6. Check which branch you are on<br/>
git branch<br/>
<br/>
or<br/>
<br/>
git branch --show-current<br/>
7. Pull latest changes first (recommended)<br/>
git pull origin <branch-name><br/>
<br/>
Example:<br/>
<br/>
git pull origin main<br/>
<br/>
Resolve any conflicts if Git reports them.<br/>
<br/>
8. Push changes<br/>
git push origin <branch-name><br/>
<br/>
Example:<br/>
<br/>
git push origin main<br/>
If Git asks for authentication<br/>
<br/>
Depending on your Git provider, you may need:<br/>
<br/>
Personal Access Token (PAT) instead of password<br/>
SSH key authentication<br/>
<br/>
For example, with GitHub, passwords are no longer accepted for Git operations over HTTPS.<br/>
<br/>
Useful commands for troubleshooting<br/>
<br/>
Check remote repository:<br/>
<br/>
git remote -v<br/>
<br/>
See commit history:<br/>
<br/>
git log --oneline -5<br/>
<br/>
See differences before committing:<br/>
<br/>
git diff<br/><br/><br/>
