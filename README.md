# Learning_Git

### Local ###

1. # Create README.md
echo "# Learning_Git" >> README.md
-> Creat Readme file (not mandatery but suggestion)

2. # Git init
git init
->Create source Git

3. # Git Status
git status
-> Check all files and folders in that specfic folder to check all the changes. 

4. # Git add 
-> Add all the NEW files or folders to local Git 
    **4.1  Git Add Url**
    git add url
    -> Url is directory of spefic files or folders that have been changed or new. 
    4.2 Git Add .
    git add .    
    -> Get all the files or folders that changes or create new

5. # Git Commit
git commit -m "messages"
->put all the files and folder that have been added to get ready to push to online Git

6. # Git Branch
git branch
->check all current work to see which branch I am at.

7. # Git Checkout -b NameOfBranch
git checkout -b nameofbranch
-> Create new branch from current branch(Master)

8. # Git Checkout NameOfBranch
git checkout nameofbranch
-> Change to another branch

9. # Git log
git log
-> check all commits

10. # Git Remote -v
git remote -v
-> Check reposisory on GitHub

11. # git remote add origin url
git remote add origin git@github.com:lekien01/Web_Development_Project.git
-> Git add local directory to GitHub
--> origin is the url. Next time just used origin instead of all url

12. # git remote -v
git remote -v
-> Check reposisory on GitHub

13. # git push origin NameofBranch
git push origin master
-> push all source to bit under branch called "master"

***git@github.com: Permission denied (publickey)***
->special github 

14. # Git Set Url
git remote set-url origin new.git.url/here
-> change current url to new url to origin(origin can be changed to other name such as lekien)

### GitHub ###

1. # Special JWT 
remote: Support for password authentication was removed on August 13, 2021.
remote: Please see https://docs.github.com/get-started/getting-started-with-git/about-remote-repositories#cloning-with-https-urls for information on currently recommended modes of authentication.
fatal: Authentication failed for 'https://github.com/lekien01/Web_Development_Project/'

    Step 1: Go to Setting
    https://github.com/settings/profile

    Step 2: Click button Develop Setting
    https://github.com/settings/apps

    Step3: Clock button Personal Access Tokens
    https://github.com/settings/tokens

    Step4: Choose Generate New Token(Classic)
    https://github.com/settings/tokens/new

    Step5: Token
    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

    Step6: Input token to url
    https://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@github.com/lekien01/Web_Development_Project

    Step7: Change current Git url to new Git url
    git remote set-url origin https://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@github.com/lekien01/Web_Development_Project

    if the first time please use add
    git remote add origin https://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@github.com/lekien01/Web_Development_Project


git config --global color.ui true
git config --global user.name "lekien01"
git config --global user.email "stephen.dinh01@gmail.com"
ssh-keygen -t ed25519 -C "stephen.dinh01@gmail.com"   

cat ~/.ssh/id_ed25519.pub
ssh-ed25519 AAAAC3NzaC1lZDI1NTE5AAAAIH97oCPliFlZlHJXi1KyBfI/lNJZpcSH5rRxqkeWDSGk stephen.dinh01@gmail.com

ssh -T git@github.com

***if we change so much they won't allow me to push it. I must use this line"
git push origin master -f