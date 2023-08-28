# Git for beginners

The main reason for the Repo existence is to have near hand all the major (and most used) git commands for new projects. Because, let's be honest, sometimes we don't remember that specific, and yet, super helpful command that we need to set up an update or complete a particular section without thinking about what we wish to do and then search for some help on the web (that usually comes with a lot no needed info at that time). So, in order to make my life easier, I used that infamous/excellent IA tool  (ChatGTP) to better explain how git commands should be implemented. You're welcome.

## Installation
 
- **Create an account at GitHub:**
   First, you need to make yourself an account at Github. You can do it so by going to [GitHub.com](https://github.com/) and signing up.

- **Install git on your computer:**
   Okay, after making sure you have created your GitHub account accordingly, then you'll need to have Git installed on your computer. You can download it from the official [Git website](https://git-scm.com/downloads) and follow the installation instructions for your operating system.

- **Set Up Your Identity:**
   Before you start using Git, you should configure your name and email address. Open a terminal or command prompt and run the following commands, replacing the placeholders with your actual information:
   
   ```
   git config --global user.name "Your Name"
   git config --global user.email "your.email@example.com"
   ```
## New Repository

-  **Create a Repository (Repo) at GitHub:**
    A Git Repo stores your project's files and version history. Go to your account, hit the New Repository button, and set up all the corresponding information. You can create the README.md file later on.


-  **Download the project to your computer**
    Go to your Repo on GitHub and copy the link to it. For example:
    ```
    https://github.com/GregoriM04/git-for-beginners.git
    ```
    
    Then open the Git bash terminal on the folder where you're going to clone the Repo. Finally, put the following command line:
    ```
    git clone + https://github.com/GregoriM04/git-for-beginners.git
    ```
    
    The last line will **Clone** all files (if there are any) to your computer up to the last version available. (It's recommended that the folder have the same name as the Repo in GitHub, that way, it'll be easier to remember where to push it).
    
    In case you already have all the files on your computer, then you be using the following command line on a terminal inside your folder's project:
    
    ```
    git init
    ```
    
    The last command will let Git know that it has to track all changes on that folder.

## Time to save some changes

- **Add Files to Staging:**
   Before committing changes, you must stage the files you want to include in the next commit. Use the following command to add specific files or all files in the directory to the staging area:
   
   ```
   git add filename     # Add a specific file
   git add .            # Add all files
   ```

- **Commit Changes:**
   Committing captures a snapshot of the staged changes with a meaningful message describing your actions. Use this command to commit your changes:
   
   ```
   git commit -m "Your commit message here"
   ```

- **Add files to Staging and Committing all together:**
   You can do both previous actions at the same time by using the following command:

    ```
   git commit -am "Your commit message here"
   ```

## More interesting commands

- **Viewing History:**
   You can view the commit history using:
   
   ```
   git log --oneline
   ```

-  **Working with Remotes:**
   Git allows collaboration by syncing repositories between your local machine and remote servers like GitHub, GitLab, or Bitbucket. You can connect your local repository to a remote repository using:

   ```
   git remote rm origin
   git remote add origin <remote_repository_url>
   git push -u origin main
   ```
   
   The first line will remove the origin from a Git repository, the second one will connect with the remote Repo, and the last will be pushing all changes to that Repo. Note: The first two lines will be needed just once.

- **Push and Pull:**
   To send your local changes to the remote repository, use:
   
   ```
   git push origin main   # Push to the "main" branch
   ```

   To get the latest changes from the remote repository, use:
   
   ```
   git pull origin main   # Pull changes into your local "main" branch
   ```

- **Branching:**
   Branches allow you to work on separate features or fixes without affecting the main codebase. To create a new branch and switch to it, use:
   
   ```
   git checkout -b new-branch
   ```

- **Merging:**
    When your work on a branch is complete, you can merge it back into the main branch. First, switch to the main branch:
    
    ```
    git checkout main
    ```
    
    Then, merge the changes from your feature branch:
    
    ```
    git merge new-branch
    ```

**And that's pretty much it, at least for now. I'll be updating with Repo based on my needs, or to fix any obvious error, so this guide remains helpful for me and all of those that may find it inrerecting enough.**