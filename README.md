# Installation and Configuration of Git

## Aim

To install and configure Git on a local system, create a local repository, and perform basic Git operations.

## 1. Introduction

Git is a distributed version control system used to track changes in files, maintain project history, and collaborate with other developers.

## 2. Software Requirements

* Operating System: Windows 11
* Version Control System: Git
* Remote Repository: GitHub
* Terminal: Git Bash

## 3. Installation of Git

1. Download Git from the official website: https://git-scm.com/
2. Run the installer and complete the installation.
3. Open Git Bash.
4. Verify the installation using:

```bash
git --version
```

## 4. Configuration of Git

Configure the username and email address:

```bash
git config --global user.name "Your Name"
git config --global user.email "your_email@example.com"
```

Verify the configuration:

```bash
git config --list
```

## 5. Creating a Local Repository

Create a project directory:

```bash
mkdir CDD-LAB-01
cd CDD-LAB-01
```

Initialize the repository:

```bash
git init
```

## 6. Performing Basic Git Operations

### Check Repository Status

```bash
git status
```

### Create a Sample File

```bash
echo "My First Git Experiment" > notes.txt
```

### Add the File to the Staging Area

```bash
git add notes.txt
```

### Commit the Changes

```bash
git commit -m "Initial commit"
```

### View Commit History

```bash
git log --oneline
```

### Create and Switch to a Branch

```bash
git branch feature
git switch feature
```

## 7. Connecting to GitHub

Connect the local repository to a GitHub remote repository:

```bash
git remote add origin https://github.com/YOUR_USERNAME/CDD-LAB-01.git
```

Verify the remote connection:

```bash
git remote -v
```

Push the main branch to GitHub:

```bash
git push -u origin main
```

Replace `YOUR_USERNAME` with your GitHub username. Ensure that the local repository has a `main` branch before running the push command.

## 8. Conclusion

Git was installed and configured successfully. A local repository was created, and basic Git operations, including initialization, staging, committing, viewing history, and branch creation, were performed.

GitHub was used to host the repository and demonstrate version control.
