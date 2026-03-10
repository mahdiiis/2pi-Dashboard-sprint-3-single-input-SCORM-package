# Pushing to a Friend's Repository

This guide explains the Git commands to push your current application to your friend's repository (`2pi-Dashboard-version_finale`) without losing the connection to your own repository.

### 1. Add Your Friend's Repository as a New Remote
```bash
git remote add friend https://github.com/oussnimo/2pi-Dashboard-version_finale.git
```
**Explanation:** Your project currently has a "remote" connection named `origin` that points to your newly created Sprint 3 repository. This command creates a **second** remote connection named `friend` and links it to your friend's repository URL. By doing this, you can easily push to your repo using `origin`, and push to your friend's repo using `friend`!

### 2. Push Your Code to the Target Repository
```bash
git push friend main
```
**Explanation:** This command tells Git to upload all your saved commits from your local `main` branch to the remote named `friend`. 

*(Note: If your friend's repository already has files in it like a README, Git might give you a warning and ask you to `pull` their changes first. If their repository is brand new and empty, it will push immediately without issue!)*
