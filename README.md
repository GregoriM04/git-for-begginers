# Git for beginners

The main reason for the repo existence is to have near hand all the major (and most used) git commands for new projects. Because, let's be honest, sometimes we don't remember that specific and yet super helpful git command that we need to to set up an update or to complete a particular section without thinking about what we wish to do and then search for some help on the web (that usually comes with a lot no needed info at that time). So, in order to make my life easier, I used that infamous/excellent IA tool  (ChatGTP) to better explain how git commands should be implemented. You're welcome.

## Installation
 
- **Create an account at GitHub:**
   First, you need to make yourself an account at Github. You can do it so by going to [GitHub.com](https://github.com/) and signing up.

- **Make yourself a profile on GitHub:**
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