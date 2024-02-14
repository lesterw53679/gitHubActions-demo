Cloned from: https://github.com/techwithtim/Microsoft-Live-Demo/tree/main

1. Go to GitHub, create an empty repo, lets call it 'gitHubActions-demo'
    my repo: https://github.com/lesterw53679/gitHubActions-demo
2. from VSCode clone the repo from devopsjourney1 to put it on local machine
    git clone https://github.com/techwithtim/Microsoft-Live-Demo.git
3. from VSCode make any changes you want to your repo, explore the yaml file in the .github/workflows folder
4. initialize the git repo, stage the files and do a first commit (open terminal and run the following commands)
    git init
    git add .
    git commit -m "first commit"
5. check the remote connection and if needed set it to your gitHub account repo
    
    git remote get-url origin

    you will notice it is pointing to the remote repository we copied it from to our local machine
    https://github.com/techwithtim/Microsoft-Live-Demo.git

    Set the remote to your own gitHub repo
    git remote set-url origin https://github.com/lesterw53679/gitHubActions-demo

6. lets explore some other git commmands

    git branch    //this will list all the branches in your project (only main at this point)
    git branch newFeature  //this will create a new branch in your local project called 'newFeature'
    git branch    // now you will see we have two branches
    git checkout newFeature  //this will activate branch 
    git branch       //see which branch is highlighted
    git checkout main  //switch back to the main branch
    git branch -D newFeature   //delete this branch, we're not going to do anything with it right now

    (we've added a file modified it since we last staged and commit, lets do that first)
    git add .
    git commit -m "first commit"

7. Push to gitHub
    git push -u origin main    // this will push all the changes to gitHub, do another commit if you wish


7. Install the GitHub actions extension for VSCode
    (this will make it easier to do work with actions from VSCode)


,

https://github.com/lesterw53679/mygitHubActions

https://github.com/en-rik/python-flask-blog.git

3. open a terminal and initialize the git repo: 
    git init
    git add .
    
    git commit -m "first commit"
    git remote add origin https://github.com/lesterw53679/github-actions-demo-withTim.git
    git branch -M main
    git push -u origin main
    git remote set-url origin https://lesterw53679@github.com/lesterw53679/github-actions-demo-withTim.git

4. 