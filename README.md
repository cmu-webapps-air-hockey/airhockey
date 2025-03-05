# Webapps Air Hockey

This repository is a web-based multiplayer air hockey game using HTML, CSS, JavaScript and Phaser, along with Django and websockets. This is a Carnegie Mellon University Webapps course team project consisting four team members: **Tyler**, **Max**, **Jacob** and **Michael**.

## Git Workflow
Please follow the simple workflow provided below for development. This repo only contains the `main`, `develop`, and feature branches. Below are the steps to help you get started, create features, and collaborate with the team.

### Branches Overview
- **`main`**: The main production-ready branch. Only stable, fully tested code will be merged here. This branch will be updated once per weeks.
- **`develop`**: The development branch. All new features are merged here before being prepared for merging into main.
- **Feature Branches**: Created from `develop` for new features. These branches are merged back into `develop` once completed.

### Getting Started

1. **Clone the Repository to Your Local Machine**:
   - First, clone the repository using the following command:
     ```bash
     git clone https://github.com/cmu-webapps-air-hockey/airhockey.git
     ```
   - Navigate to the project directory:
     ```bash
     cd airhockey
     ```

2. **Pull Latest Changes from `develop`**:
   - Before you start working, make sure you have the latest changes from `develop`:
     ```bash
     git checkout develop
     git pull origin develop
     ```

### Creating a Feature Branch

1. **Create a New Feature Branch**:
   - Always create a new branch from `develop` for your feature. Use the following commands:
     ```bash
     git checkout develop
     git pull origin develop
     git checkout -b feature/<your-feature-name>
     ```

2. **Work on Your Feature**:
   - Make the necessary changes for your feature.
   - Commit your changes regularly with clear and concise messages:
     ```bash
     git add .
     git commit -m "Feature <your-feature-name>: <commit-message>"
     ```

3. **Push Your Feature Branch**:
   - Once you're done working on your feature, push your branch to GitHub:
     ```bash
     git push origin feature/<your-feature-name>
     ```

### Creating a Pull Request (PR)

1. **Create a Pull Request to Merge into `develop`**:
   - Go to the repository on GitHub.
   - Click on **"Compare & pull request"** for your feature branch.
   - In the PR description, explain what the feature does and any relevant details.
   - Assign at least **2 teammates** to review your PR.
   - Select the `develop` branch as the base and your feature branch as the compare branch.

2. **Get Reviews and Approval**:
   - Once the PR is created, your teammates will review the code. You’ll need at least 2 approvals before you can merge.
   - If changes (comments on your PR) are requested, make the changes and push the updates to your feature branch. The PR will automatically update.

3. **Merge the Pull Request**:
   - After receiving the required approvals, you can merge the PR. Use the **"Squash and Merge"** option to ensure clean commit history.
   - **Do not merge directly to `main`**; all changes must go through `develop`.

4. **Delete Your Feature Branch**:
   - Once the PR is merged, delete your feature branch both locally and remotely:
     ```bash
     git branch -d feature/<your-feature-name>
     git push origin --delete feature/your-feature-name
     ```

## Summary of Commands:

- Clone the repo (only for the first time):
  ```bash
  git clone https://github.com/cmu-webapps-air-hockey/airhockey.git
  cd airhockey
  ```
- Pull the latest `develop`:

  ```bash
  git checkout develop
  git pull origin develop
  ```
- Create a feature branch from `develop` (for example, a login page):

  ```bash
  git checkout -b feature/login-page
  ```

- Happy Coding!

- Commit your changes:

  ```bash
  git add .
  git commit -m "Feature login-page: Add super awesome button"
  ```

- Push your feature branch:

  ```bash
  git push origin feature/login-page
  ```

- Create a Pull Request (PR) from `feature/login-page` to `develop`.

- Merge the PR into `develop` (after review and approval).

- Delete your feature branch:

  ```bash
  git branch -d feature/login-page
  git push origin --delete feature/login-page
  ```

- `develop` will be merge into `main` every week (with approval fromall team members)