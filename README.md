# TestingRepo- Just for learning purposes. Will be deleted afterwards

# Rules
- Use clean code principles :
  - use relevant naming 
  - use simple function (every function does one thing)
  - write specifications (where we can't understand from the first reading what the function is doing)
  - distribute functions into files (at most 10 functions per file) 
- We will use github projects for management. 
  - You will see if you go into [Projects](https://github.com/TheXGeneral/Unihack_before/projects) tab. 
  - There, go on the project that has the same name as you predefined branch that you are working on. 
  - There you'll see multiple columns(To do, Doing, Done) with card looking elements. You can move those elements and show everybody what are you working on.  
  - Try to have only one task in doing in the same time 
  - After you finished a task, push you code into a branch, await for merge and then, move the task into the Done column. 
  - Don't do more tasks on a single branch. We don't want kebab branches (cu de toate)
  - Name you commit and your branch after the task that you done
- There is a rule in programming. Main branches need to always work. If your code has errors that make code to crash, don't request a merge into a predefined branch 

# Git tutorial 
- This can be used in github desktop, but I don't have any experience with it untill now, so I will put here commands for Git Bash (console version of git)
- More complex documentation about git: https://devconnected.com/category/software-engineering/
- Please ask before doing something stupid :)))
- Download:   https://git-scm.com/downloads

1. Clone a repo 
      ```
      git clone https://github.com/TheXGeneral/Unihack_before.git
      ```
      - That link is obtained by clicking `Code` button and selecting https link. This will display a link used for cloning.
      - For cloning a repo. right click in the folder you want to have your repo. In the menu that poped up, select git bash. A console simillar to cmd will pop up. put the command in it.
      - For any other commands, it's enough to get into the repo's folder, and in the folder bar to write cmd. this will pop up a command promt console. There, you can run any command you want
2. Add command ( used when preparing to push changes )
      ```
      git add . 
      ``` 
      - This will be used to add all packages not previously added on git 
      
3. Commit 
      ```
      git commit -m "commit message"
      ```
4. Push 
      ```
      git push origin <branch_name>
      
      -----for example------
      git push origin master 
      git push origin br1
      ```
      - In order to completely push something to github, you need to add, commit and push
5. Pull changes from github
      ```
      git pull
      ```
6. working with branches
      - What is a branch: another code base that does not interfere with the main one. I can keep one code into the main branch and another code into other branches.
      - When you pull must happen on the main branch. Any work that you do will happen on the branch that is keeping that code.
      - Moving between branches:
      ```
      git checkout <existing_branch>
      
      --for example --
      git checkout main
      ```
      
      - Moving on a branch and creating that branch ( to be called only when you want to work on a different branch than the ones predefined)
      ```
      git checkout -b <new_branch>
      
      --for example -- 
      git checkout -b my_new_branch
      ```
      - Move to main to pull data and after that, move back to your branch
7. Special push 
      - This push also creates a new branch when pushing. You will work on one of the predefined branches
      - When pushing code, to make sure that there are not any conflicts, push to a different branch, usually named after the task you done
      ```
      git push origin HEAD:API_branch_added_tests 
      ----- on github, you'l see that a new branch was created and your code is on it -----
      ```
      - After that you will have to merge your branch into one of the predefined branches, but this will be done with help from me ( this opperation might result in serious harms to the code base, so, because you don't have experience with it, I will help you)
