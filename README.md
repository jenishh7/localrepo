# Repository Initialization and Management

## Initialize the Repository

To start a new repository, follow these steps:

1. Initialize a new Git repository:

   ```bash
   git init
   ```

2. Add a remote repository:

   ```bash
   git remote add origin <Link>
   ```

3. Verify the remote repository configuration:

   ```bash
   git remote -v
   ```

4. Check the current branch:

   ```bash
   git branch
   ```

5. Rename the current branch to `main` (if needed):

   ```bash
   git branch -M main
   ```

6. Push the changes to the remote repository:
   ```bash
   git push origin main
   ```
   Alternatively, you can use:
   ```bash
   git push -u origin main
   ```

## Add and Push Changes

To add and push changes to the repository:

1. Stage all changes for commit:

   ```bash
   git add .
   ```

2. Commit the changes with a meaningful message:

   ```bash
   git commit -m "Your message here"
   ```

3. Push the committed changes to the remote repository:
   ```bash
   git push origin main
   ```
   If you used `-u` in the initial push, you can simply use:
   ```bash
   git push
   ```

## Branch Commands

To manage branches, use the following commands:

1. **Check the current branch:**

   ```bash
   git branch
   ```

2. **Rename the current branch to `main`:**

   ```bash
   git branch -M main
   ```

3. **Navigate to a different branch:**

   ```bash
   git checkout <branch name>
   ```

4. **Create a new branch and switch to it:**

   ```bash
   git checkout -b <new branch name>
   ```

   Example:

   ```bash
   git checkout -b feature1
   git branch
   git checkout main
   git checkout -b feature2
   git branch -d feature2   # Note: You cannot delete the branch if you are currently on it.
   ```

5. **Delete a branch:**
   ```bash
   git branch -d <branch name>
   ```

## Merging Code

To merge code from one branch into another:

### Way 1: Command Line

1. **Compare branches, commits, files, etc.:**

   ```bash
   git diff <branch name>
   ```

2. **Merge the branches:**
   ```bash
   git merge <branch name>
   ```

### Way 2: Pull Request (PR)

1. **Create a Pull Request (PR) on GitHub:**
   - Go to your repository on GitHub.
   - Navigate to the "Pull Requests" tab.
   - Click "New Pull Request."
   - Select the branch you want to merge into (base) and the branch you want to merge from (compare).
   - Review the changes and submit the Pull Request to let others review and discuss your changes before merging.
