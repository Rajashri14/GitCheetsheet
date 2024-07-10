
Git commands cheatsheet :-

1. git init-----> powers your folder to be managed by git and initiates a new empty repository. 
               It also creates a .git folder that has all the relevant logic to manage versions of your project

2. rm -rf .git---> removes .git folder . If we don't want to track changes anymore by git.

There are 3 areas in which your file changes are done--->

1) Working area---> There can be bunch of files that are not currently handled by git.
                    It means that changes done or to be done in those files are not managed by git yet.
                    A file which is in working area is considered to be not in the staging area.
                    When we do `git status` and we see a bunch of `untracked files` then these are actually 
                    called to be in working area

2) Staging area----> What all files are going to be part of the next version that we will create.
                     This staging area is the place where git knows what changes will be done from the last version
                      to the next version.

3) Repository area---> This area actually contains the details of all your previous registered versions.
                       And the files in this area, git already manages them and knows their version history.



 3. `git add <file_name>`----> moving untracked files from the working area to the staging area

 4. `git rm --cached <file_name>`----> moving files from staging area back to working area

 5. `commit `----> is a particular version of the project.It captures a snapshot of the project's staged changes and creates a version out of it.

6. `git clone`----> cloning repositoryy on our local machine
               git clone <some link>

7. `git commit`----> it will open vim editor
                  press i and type the commit message 
                  press esc the colon to save the changes 
                  press wq to exit the vim editor.

8. `git log`----> this command list all the commits and details about them.(every commit have unique commit id using we can go back to that
               particular commit.

9. `git restore <file_name>` ----> it removes all files changes from the statging area to be committed.
                                This can be useful if did some dirty piece of code and now no more want it.
                                Instead of deleting every change line by line, we can restore it or you can say last clean version of 
                                the files can be restored.

10. `git restore --staged <file_name>`----> it removes file from changes from staging area to the working area.
                                      this only works if changes are in your statging area.

11. `git diff commit1id commit2id`----> gives the difference of all the file changes between two commits

12. `git commit -m "<your commit message>"`----> If we want to avoid opening a text editor like vim/nano to add commit message we can use this command.

13. `git remote`---> list down all the remote connection names

Remote Connection :----> It helps you to link to git repositories for uploading and downloading changes from each other

14. `git remote add <name of the remote connection> <link of the remote>`-----> this command helps us to add a new link to the remote repo and give a name to it.

15. `git remote rm <name of remote>`----> this command deletes a remote connection

16. `git remote rename <old_name> <new_name>`----> this command renames the remote connection

Note: The name of the remote connection is always used to establish communication between repos

17. `git push`---> upload local repo content to remote repo
            git push origin 
            

ls --> list the files in current directory
la -a ---> list all the files (hidden files also)



            

