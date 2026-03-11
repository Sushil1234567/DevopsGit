**** GIT COMMANDS CHEATSHEET ***

======================================================================================SETUP & CONFIG COMMANDS====================================================================================================




git init : used to initialize (or create) an empty git repository in the current directory . This prepares the directory for version control by creating a hidden folder: .git , which stores all the configura-             tion files Hence the directory can be considered as a git repository hence forth post git init

           Example : (navigate inside the directory)
                     RUN: git init 



git config --user.name "<name>" : this is used to SET the name of the author at local level (for the current repository)

                                  Example: git config --user.name "myname"

git config --user.email "<email>" : this is used to SET the email id of the author at local level (for the current repository)
                                     
                                    Example: git config --user.email "xyz@mail.com"





git config --global user.name "<name>" : this is used to SET the name of the author at global level (for all the repositories)

                                         Example: git config --global user.name "myname"

git config --global user.email "<email>" : this is SET to set the email id of the author at global level (for the current repositories)

                                           Example: git config --global user.email "xyz@mail.com"




git config --user.name : this is used to CHECK the name of the author at local level (for the current repository)

                         Example: git config --user.name    [o/p: displays name of the author for the current repository]

git config --user.email : this is used to CHECK the email id of the author at local level (for the current repository)

                          Example: git config --user.email  [o/p: displays email of the author for the current repository]




git config --global user.name : this is used to CHECK the name of the author at global level (for all the repositories)

                                Example: git config --global user.name   [o/p: displays name of the author for all the repository]


git config --global user.email "<email>" : this is used to CHECK the email id of the author at global level (for the current repositories)

                                           Example: git config --global user.email   [o/p: displays name of the author for all the repository]








======================================================================================BASIC WORKFLOW COMMANDS=====================================================================================================


git status: DISPLAYS the current branch name and  the information regarding the status of any file created i.e untracked, modified, or pending commit, this is used frequently to check the state of the project
      
            Example: git status [ displays details regarding state of the project/repository ]


git add <filename> : used to STAGE all the changes made in file 
               
                     Example: git add filename.txt 


git commit -m "description" : used to COMMIT the staged changes by provding some message about the change 

                              Example: git commit -m "Info.about the changes"


git log : SHOWS the commit history of the current branch
         
          Example: git log


git branch < branch_name > : used to CREATE a new local branch 
       
                             Example: git branch enterbranchname 

git branch : used CHECK the current branch 

             Example: git branch


git checkout -b < branch_name > : creates a new branch and switches to it 
               
                                  Example : git checkout -b dev 
                                            user will be checked out to a new branch 'dev' as current branch.


git checkout < branch_name > OR git switch < branch_name > : used to switch between two branches .
                          
                                                             Example: suppose we are in branch dev , inorder to make any changes in branch main, do 
                                                                      git switch main    ;user will enter branch: main



git merge < branch_name > : combines changes from the specified branch into our current branch

                            Example: git merge dev 
                                     incase we want to merge the changes of dev branch to the current branch(main);
                                     from current(main) branch run: git merge dev
                                     this will combine all the changes in the main branch to the current branch.



git pull origin < source >: fetches the changes the remote repository  and merges into our current local branch

                            Example: if there is a need to obtain the changes that are in the remote repository , and we need to merge them into our local repository , run
                                     git pull origin main

git push origin < source >: uploads the local commits to the main  or remote repository 
                           
                            Example: after making a new change in our local , which is not present in the main repository, we push the changes 
                                     git push origin main









