# git-notes

## Creating a repo and linking it to a remote

### With a fully configured remote

 1. Create the remote in GitHub
 1. Ensure there is at least one commit in the remote
 1. Copy the remote SSH URL from the repository on GitHub
 1. `git clone <remote--ssh-url>`

### Linking an existing local repository to an existing remote

 1. Create the remote in Github
 1.  Ensure there is at least one commit in the remote
 1. Create the local repository: `git init`
 1. Rename the local repository to main, if using GitHub: `git 
branch -m main`
 1. Commit something to the local branch to initialize it.
 1. Configure the remote: git remote add origin <ssh string 
copied 
from GitHub>
 1. Tell git how to resolve branch divergence: `git config 
--global pull.rebase true`
 1. Pull down the information from the remote: `git pull origin`
 1. Set upstream for the local branch: `git branch -u origin/main 
main`
