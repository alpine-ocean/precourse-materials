# GIT

## QUESTIONS

- What is git? Why do we need it?

    git is an open source revision control system. It is needed
    to collaborate effectively. Also providing the ability to revert to earlier versions if needed. 

- What are the top 10 commands? What do they do?

    1. git clone <https://name-of-the-repository-link> 

        Copies a repository from an online source locally and initiates a local git repository.

    2. git branch <branch-name>

        Creates a branch of a local repository, so that you can 
        work on a feature in parallel to main. 

    3. git checkout <branch-name>

        Switches branches. Two things to keep in mind: 

            - Any changes in the branch you are currently working
            in need to be committed or stashed before switching to
            a new branch.
            - The branch you are switching to should already exist.

        You can combine commands git checkout -(b)ranch <branch-name>
        to create and switch to the branch just created.

    4.  git status

        returns whether: 
            
            - the current branch is up to date
            - there is anything to commit, push, or pull
            - there are files staged, unstaged, or untracked
            - there are files created, modified, or deleted

    5. git add <>

        This command stages files for the next commit. If they aren't staged
        first with this command, they will not be included. 

    6. git commit <>

        This command creates a snapshot in the repository that you can revert
        to if needed. You can add a -m flag to include a message. A message should always be included. I currently have my git set up to open a new 
        window to write proper commit messages. I can't remember how I did that, 
        but it was something I learned to configure through TOP "The Odin
        Project."

    7. git push <>

        This command pushes anything that has been committed to the online
        repository.

    8. git pull <>

        This command gets updates from the remote repository. However its a
        combination of git fetch and git merge, so the command both fetches and
        merges any changes with what you have locally which can sometimes cause
        issues requiring manual conflict resolution. 

    9.  git revert <hash of commit>

        This command allows you to safely revert to a prior commit without
        deleting anything. It creates a new commit of the selected previous
        commit while retaining all commits in between. 

    10. git merge <branch-name>

        Merges your feature branch into the parent branch. You first need to be
        on the parent branch before running this command. BEst practice is to use git fetch <parent-branch> to make sure it is up to date, then you can
        safely run git merge. 

- How do you open a PR?

    After pushing changes to github, go to the repository on github and follow the prompts.

## RESOURCES

GIT Cheatsheet:
https://education.github.com/git-cheat-sheet-education.pdf
https://www.freecodecamp.org/news/10-important-git-commands-that-every-developer-should-know/

Commands:
https://www.techrepublic.com/article/16-terminal-commands-every-user-should-know/

Bash vs zsh:
https://www.howtogeek.com/68563/htg-explains-what-are-the-differences-between-linux-shells/

What's the difference?
https://askubuntu.com/questions/506510/what-is-the-difference-between-terminal-console-shell-and-command-line