# To use git for your project, you need to:
1. configure git.
    **Tell git who you are**: 
        `git config --global user.name "Your Name"
        `git congig --global user.email "youremailaddress"
    **Check the username and email**:
        `git config user.name`
        `git config user.email`
    **View all settings**:
        `git congig --list`
    
2. initialize your repository.
    **Initialize git in your project**:
        navigate to your project folde, make sure you are inside your project folder
            `cd path/to/your/project-folder`
        initialize git to start tracking this folder
            `git init`
        set your default branch name 
            `git branch -M main`
        check what git is tracking and make sure it is working
            `git status`
        check which branch you are on
            `git branch` or `git status`
    set your default branch to main before using `git init`
        `git config --global init.dafaultBranch main`
        it sets a permanent rule for future.
    If you have already used git init:
        use `git branch -M main` to fix the current repository.
        this works only for this specific folder.
3. save your files locally.
    **Saving your progress is a two-step process**
    1. check the status to see what files git detects:
        `git status`
    2. stage all your files to prepare them for saving(next commit)
        `git add .`
    3. commit the files with a descriptive note called message
        `git commit -m "Initial commmit: Add project files"`
    
4. push them to github.
    **Link your local project to github"
    create a new repository on github
    copy paste the command from github to your terminal to push an existing repository from the command line








## Daily Git Workflow After Setup
- `git add .` -> Stages all new changes.
- `git commit -m "Explain your changes"` -> Saves a snapshot locally.
- `git push` -> Uploads the changes to GitHub.
