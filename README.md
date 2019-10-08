# githelp

### git init => to setup git

### git add file_name => to add file to staging area

### git log => to view logs of commits made

### git commit -m "commt message" 

### git add . => to add all files to staging area

### git status => to view git status of all files

//#### FILE IN/OUT in STAGING AREA ##### //

1. changed something in index.html then if you need to go back to previous or original state then enter

    -  git checkout index.html
    
2.  To revert back changes from staging area

    -  git reset HEAD index.html  (removes changes in staging area), then git add . git commit
    
3.  File deletion

     -  Delete a file from code then bring it back through git
       - git checkout about.html (deleted file from code)
     - To push delete in stageing
       git add about.html ( file delted from git) 
       git reset HEad about.html ->git rm about.html ( revert back delete and then delete the file in fast way)
      
 //#### LOG ##### //
 1.  To move back to prevous or any commit made
 
     -  git log -> list all longs & hash code -> git checkout hashcode ( hashcode of the commit you want to revise/ redo) if you commit any thing at this stage, you will have a branch with that name like *(head detached) / master, you can move back to master to view the orginial commites which are made before git checkout hashcode
     
 2. To create new branch
 
     -  git branch branch_name
     
 3. To create a branch for a old commit or head change
 
     -  git branch branhc_name hashcode(bc272745) (i.e)  *(head detached) / master
     
 // #### Controlling state with branch ### //
 
 1.  git branch  => will list all branches
 
 2. To move to new brnach => git branch branch_name (existing branch name)
 
 3. Merge to other branch to master
 
     -  git merge branch_name ( you have to be in master branch as current branch while doing this command)
     
 4. Change branch name:
 
     - git branch -m old_branch_name new_branch_name
     
 5. To remove Branch:
 
      - git branch -D branch_name
  
  // ### Git hub project download ### // 
    > PWD will show current directory
  
  1.  Clone git
      
      - git clone url_of_github  (clone master branch)
   
  2. To View all branch & clone a branch from github (origin)
  
      -  git branch -a
      -  to clone branch from origin => > git checkout -b local_branch_name origin_branch_name
      
  3. To clone all branches from origin
      
      -  > git clone --mirror url_of_git .git
      -  after that > git config --bool core.bare false
      -  after that > git reset --hard
      
 
 
