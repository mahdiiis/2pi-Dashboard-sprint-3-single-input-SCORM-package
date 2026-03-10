# Repository Migration & Push Guide

This document explains the Git commands used to push your current project from the old repository (\`sprint-2\`) to the new one (\`2pi-Dashboard-sprint-3-single-input-SCORM-package\`).

### 1. Stage All Changes
```bash
git add .
```
**Explanation:** This command tells Git to track all the file changes, additions, and deletions you've made in the project directory, adding them to the "staging area" to be ready for an official commit.

### 2. Commit the Changes
```bash
git commit -m "feat: complete sprint 3 single input and SCORM package updates"
```
**Explanation:** This command permanently records the staged changes in your local Git repository's history along with a descriptive message.

### 3. Update the Remote Repository URL
```bash
git remote set-url origin https://github.com/mahdiiis/2pi-Dashboard-sprint-3-single-input-SCORM-package.git
```
**Explanation:** In Git, \`origin\` is the default name for the remote server you push to. Since this project was cloned from the Sprint 2 repository, \`origin\` still points there. This command updates the \`origin\` URL so that it points to your **new** Sprint 3 repository on GitHub.

### 4. Push to the New Repository
```bash
git push -u origin main
```
**Explanation:** This command uploads all your local commits to the new remote repository. The \`-u\` flag tells Git to set up tracking, linking your local \`main\` branch with the remote \`main\` branch. Now, any future \`git push\` commands will automatically know where to go without having to specify \`origin main\`.
