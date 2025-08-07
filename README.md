# ALXprodev-advanced_git

This repository demonstrates advanced Git usage as part of the ALX Professional Developer program. It follows GitFlow branching strategy and includes automated Git hooks for ensuring consistency and improving team collaboration.

## 📁 Project Structure

```

┣ 📂hook-test-folder
┃ ┣ 📜README.md — Description of the test folder used to validate the pre-commit hook
┃ ┗ 📜sample.txt — A test file
┣ 📂login-page
┃ ┗ 📜README.md — Documentation for the login page component
┣ 📂signup-page
┃ ┗ 📜README.md — Documentation for the signup page component
┗ 📜README.md — This file

````

## ⚙️ Git Hooks Implemented

### ✅ Pre-commit Hook
- **Purpose**: Ensures that every subdirectory in the repository contains a `README.md` file.
- **Behavior**: Prevents commits if any directory lacks a `README.md`, maintaining documentation standards.

### ✅ Post-merge Hook
- **Purpose**: Logs all successful merges into the `main` branch.
- **Behavior**: After merging into `main`, a log entry is appended with details about the merge.

## 🌱 GitFlow Branching

This repository uses the [GitFlow workflow](https://www.atlassian.com/git/tutorials/comparing-workflows/gitflow-workflow):
- `main`: Stable production-ready code
- `develop`: Active development branch
- `feature/*`, `release/*`, `hotfix/*`: Temporary branches for specific GitFlow tasks

## 🛠️ Getting Started

To clone the project and use the Git hooks:

```bash
git clone git@github.com:HabtamuTesafaye/ALXprodev-advanced_git.git
cd ALXprodev-advanced_git

# Make sure Git hooks are executable
chmod +x .git/hooks/pre-commit
chmod +x .git/hooks/post-merge
````
