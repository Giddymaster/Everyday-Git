# Everyday Git

## What is Git?
Git is a version control system that allows you to manage and track changes in your source code. It is a distributed version control system, meaning that the entire codebase and history are available on every developer's computer, allowing for easy branching and merging.

### Benefits of Version Control System (VCS):
- Keep track of changes in the code.
- Collaborate with other developers.
- Revert to previous versions in case of errors.
- Work on different features simultaneously without conflicts.

## Installing Git
Before you start using Git, install it on your computer and configure it with your name and email address.

1. Download Git from [Git SCM](https://git-scm.com/).
2. Confirm installation by running:
   ```sh
   git --version
   ```

## Configuring Git
To configure Git with your name and email, run:
```sh
git config --global user.name "Your Name"
git config --global user.email "your_email@example.com"
```

## Creating a New Repository
1. Navigate to your project directory in the terminal.
2. Initialize a new Git repository:
   ```sh
   git init
   ```
3. Check the status:
   ```sh
   git status
   ```

## Adding Files to the Staging Area
To add files before committing:
```sh
git add filename   # Adds a specific file
git add .          # Adds all files
```
Check status using:
```sh
git status
```

## Committing Changes
Save changes with a commit message:
```sh
git commit -m "Initial commit"
```

## Working with Branches
Branches help manage different lines of development within a project.

### Creating a Branch
```sh
git branch branchname
```

### Viewing All Branches
```sh
git branch
```

### Switching Branches
```sh
git checkout branchname  # Older method
git switch branchname    # Recommended method
```

### Merging a Branch
```sh
git merge branchname
```

### Deleting a Branch
```sh
git branch -d branchname  # Delete local branch
git push origin --delete branchname  # Delete remote branch
```

## Working with GitHub
### Creating a GitHub Repository
1. Go to [GitHub](https://github.com/new).
2. Click "New repository".
3. Enter details and create the repository.

### Adding a Remote Repository
Copy the remote repository URL and run:
```sh
git remote add origin <repository-url>
```

### Pushing Changes to GitHub
```sh
git push origin branchname
```

## Collaboration with Git
- Clone a repository:
  ```sh
  git clone <repository-url>
  ```
- Fetch and merge changes:
  ```sh
  git pull
  ```
- Push changes:
  ```sh
  git push origin branchname
  ```

## Next Steps
- Learn about GitHub workflows (Git Flow, GitHub Flow, etc.).
- Explore advanced Git commands (rebasing, cherry-picking, stashing).
- Collaborate on open-source projects.
- Automate tasks using Git hooks.
