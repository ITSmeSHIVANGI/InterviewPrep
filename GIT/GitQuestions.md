# BASICS

## Daily used Commands
1) Clone : copy the repository[default branch] into the local system.
    git clone [Repo link]

2) Switch between branches: only works when both the branch exists in local
    git switch [branch name] ==  switch to mentioned branch
    git switch - == switch to previous branch

3) Fetch remote branch locally
    git fetch
    git switch -c [branch name] origin/[branch name]

4) Create a new branch
    git switch -c [branch name]

5) Push to remote
    a) git add . or  git add [filename]
    b) git commit -m " COMMIT MESSAGE " 
    c) git push origin [branch name]

6) Pull from remote
    a) git fetch == all the changes from all commits by other users comes locally but doesnot merge into the local branch which u r currently working on 
    b) git pull origin [branch name] == merges all the remote changes into the local branch.

7) git rebase 
    example of rebase 

    a) main branch -  this contains commits as A,B,C
    b) branch B -  replica of branch main -  also got the coomits A,B,C
    c) a few more commits get added to the main branch  i.e 1,2,3
    d) on the branch B a few commits added i.e E,F,G

    Problem : on the branch B the commits required as A,B,C 1,2,3,E,F,G

    Solution : git rebase

    1) switch to main branch
    2) git reset --hard
    3) git fetch 
    4) git pull origin main  == now we habe commits till A,B,C,1,2,3
    5) switch to Branch B
    6) git rebase main == now all the changes are as A,B,C,1,2,3,E,F,G LOCALLY
    7) git push -f (force)

8) 



   
## More Topics
1) Git Status ->
2) Git add . ->
3) git restored -> View all the commits made in the history
4) git stash
5) squash

Fork VS Branching, which one to use
What is Git? How is it different from other version control systems?
Ans : 
What is the difference between Git and GitHub?
What is a repository in Git?
What is the difference between a local and remote repository?
What is git init and what does it do?
What is git clone? How is it different from git init?
What are the three stages in Git? (Working Directory, Staging Area, Repository)
What is git add and what does it do?
What is git commit and why is it important?
What is git status used for?
What is git log? What are some useful flags with it?
What is .gitignore? Why is it used?
How do you undo the last commit without losing changes?
What is the difference between git pull and git fetch?
What is git push and how does it work?


