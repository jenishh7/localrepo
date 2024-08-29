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
