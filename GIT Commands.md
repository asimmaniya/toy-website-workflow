Version control is also sometimes called source code management, or SCM.

Track the changes you make to a file.
View the history of a file, and go back to an older version if you need to revert a change you've made.
Work with multiple versions of a file at the same time.
Collaborate with other team members by sharing your code and changes.
distributed version control system

# Check the installed version of Git
git --version

# Configure the global user name for Git commits
git config --global user.name "USER_NAME"

# Configure the global email address for Git commits
git config --global user.email "USER_EMAIL_ADDRESS"

# List the current Git configuration
git config --list

# Initialize a new Git repository
git init

# Show the status of the repository, including staged and unstaged changes
git status

# Rename the current branch to "main"
git branch -M main

# Stage the changes in the specified file
git add deploy/modules/cosmos-db.bicep

# Stage all changes in the repository
git add .

# Create a new commit with the staged changes and provide a commit message
git commit --message "Add Cosmos DB account definition"

# Show the commit history, with each commit on a single line
git log --pretty=oneline

# Show the commit history for a specific file
git log deploy/main.bicep

# Create a new branch named "my-experimental-changes" and switch to it
git checkout -b my-experimental-changes

# Switch back to the "main" branch
git checkout main

# Merge the changes from the "my-experimental-changes" branch into the current branch
git merge my-experimental-changes

# Delete the branch named "my-experimental-changes"
git branch -d my-experimental-changes

# Add a remote named "origin" with the URL of your repository
git remote add origin YOUR_REPOSITORY_URL

# List the configured remote repositories
git remote -v

# Push the local branch "main" to the remote repository named "origin" and set it as the upstream branch
git push -u origin main