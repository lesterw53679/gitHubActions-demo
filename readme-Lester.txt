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

8. Pull from remote  (first make some changes to the repo in GitHub, like add a readme file) 
    git pull origin main

9. Branching:  Lets try branching and doing a pull request
    git checkout -b changeBranch
 (now we are local and sitting on the "changeBranch" branch, make some modifications to files)

    git add .
    git commit -m "branch example commit 2"
    git push origin changeBranch


10. Merge Branch: Go back to GitHub and do a compare and pull, this will trigger the action because we are doing a pull and compare on this

    select the branch you want to merge into the main branch
    compare the differences, check that we have successfully passed all the tests

 11. Bring your local project up to date:
    git pull origin main    //now your local is up to date, merged branches

    if you need to delete the branch manually:
    git branch -D changeBranch

12. Note on doing matrix
on: [push, workflow_dispatch]
    branches: [main, prod]
   
   branches:
      - "main"  
      - "prod"


13. Install the GitHub actions extension for VSCode
    (this will make it easier to do work with actions from VSCode)
14. Break the code, raise Exception()

Links:
GitHub Docs: https://docs.github.com/en/actions
GitHub Guides: https://docs.github.com/en/actions/guides
GitHub Actions Repo: https://github.com/actions
GitHub Azure Actions Repo: https://github.com/Azure/actions

UDEMY:  Highly recommended

Maximilian Schwarzmüller (instructor) 
https://www.udemy.com/course/github-actions-the-complete-guide/#instructor-2
https://www.udemy.com/course/github-actions-the-complete-guide/


Coder Dave GitHub: https://github.com/n3wt0n
Coder Dave GitHub Actions demo: https://www.youtube.com/watch?v=TLB5MY9BBa4

Uses VSCode:
Tech With Tim GitHub: https://github.com/techwithtim
Tech With Tim GitHub Actions video: https://www.youtube.com/watch?v=UEOtZvTCmDo

Alfredo Deza Run Python in GitHub Actions: https://www.youtube.com/watch?v=o2o_xF6NhD0

TechWorld with Nana GitHub Actions CI/CD: https://www.youtube.com/watch?v=R8_veQiYBjI&t=121s

glitch.stream GitHub Actions full course: https://www.youtube.com/playlist?list=PLArH6NjfKsUhvGHrpag7SuPumMzQRhUKY

Uses VS Code:
Dev Leonardo Understanding GitHub Actions - Automated Testing
https://www.youtube.com/watch?v=WW6ZUw9IExA&t=2s


Software Engineer Tutorials: How To Use GitHub + VSCode: Create a Repository & Merge Changes With a Pull Request
https://www.youtube.com/watch?v=eLmpKKaQL54&t=363s

Another Video GitHub + VSCode: https://www.youtube.com/watch?v=mR9jhYD3bnI

**Harsivo Edu: GIT with VSCode - Pull and Create New Branch | GIT Pull & Git Create new Branch
https://www.youtube.com/watch?v=hyLAfceeM1E

Harsivo Edu: Playlist for Git and GitHub:  https://www.youtube.com/watch?v=lYiE5lBS13E&list=PLo7aAWjVsGnED1--V1cn1_VE4a8btkL-l

Azure Deployment
Milan Jovanovic:  How To Deploy Your Application To Azure Using GitHub Actions | CI/CD Pipeline
https://www.youtube.com/watch?v=QP0pi7xe24s&t=3s
His Playlist:
https://www.youtube.com/@MilanJovanovicTech/videos

How to get started with GitHub Actions for Azure | Azure Tips and Tricks:
https://www.youtube.com/watch?v=zcYqejz6Iig
