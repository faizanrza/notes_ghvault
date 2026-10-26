# To use git for your project, you need to:  
1. configure git.  
    **Tell git who you are**:   
        `git config --global user.name "Your Name"`  
        `git config --global user.email "youremailaddress"`  
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
    and follow the instructions given there to push your project.  
    `git remote add origin https://github.com/your/repo/url`  
    `git branch -M man`  
    `git push -u origin main`  
    all these are one time commands you only need to use then when you pushing for the first time.  

    If you set up wrong link then fix it:  
        `git remote set-url origin https://github.com/correct/link`  

        Verify the online address the git is pointing to:  
        `git remote -v`  


## Daily Git Workflow After Setup  
- `git add .` -> Stages all new changes.  
- `git commit -m "Explain your changes"` -> Saves a snapshot locally.  
- `git push` -> Uploads the changes to GitHub.  


## Check Status of commits and pushes and other things  
- `git status` : to see If you have unpushed work or uncommited changes.  
- `git log` : to see a timline of all your commits.  
    `git log --online` : more readable.  
- `git diff` : to see the exact code edits you made.  