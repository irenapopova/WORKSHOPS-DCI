### Basic Commands
#### 👉 🛑 Git Config :
 **`git config -- global user.name NAME`** = set user name globally
**`git config --global user.email EMAIL`** = set user email globally
**`git config user.name || git config user.email `** = check saved info

#### 👉 Creating repo
**`git init `** = creates a git repository in the directory currently in

#### 👉 Staging 🤔 
**`git status `**= to check status , if staged or unstaged
**`git add FILE_NAME `**= to add a file to staging area
**`git rm --cached FILE_NAME `** = to remove a file from staging area
**`git add . `** = to add all files in project to staging area

### 👉 Commiting
**`git commit -m "Specific Changes Made" `**= commits the staging area giving them a specific id

**`git log `**= shows all the commits with details

**`git log --oneline `**= shows all the commits in one line each

🛑 SPECIAL log : this will log the info in a nice format (Try it once 😉)
**`git log --graph --pretty=format:'%Cred%h%Creset -%C(yellow)%d%Creset %s %Cgreen(%cr) %C(bold blue)<%an>%Creset' --abbrev-commit  `**   
this can be used as an alias

### 👉 Git Stash
**`git stash`** = clears the changes to the initial state (last commit) & creates a unique id for the current state
**`git stash apply`** = brings back the current state
using git stash multiple times creates a list of stashes of all states with multiple ids
**`git stash list`** = shows all the stash (States) with their ID
**`git stash apply ID `**= ID will be the number , which state you want to go back to
**`git stash push -m "Your message"`** = used to give description to stash
**`git stash drop ID `** = used to remove a stash saved
**`git stash pop ID `**= applies the specific stash and removes it from history
**`git stash clear `** = removes all the stash history
