Global Config

Use ssh key, 
Project with Git  
========================

Command line, code, etc

Show all settings

    git config -l 

1) Global -  Config
----------------------------------
    rerere.enabled=true
    push.default=current
    user.name=mventura
    user.email=mventura@mail.com
    color.ui=true
    merge.tool=meld
    editor=vi
    core.repositoryformatversion=0
    core.filemode=true
    core.bare=false
    core.logallrefupdates=true
    remote.origin.fetch=+refs/heads/*:refs/remotes/origin/*
    remote.origin.url=git@github.com:vpg/yourproject.git


2) Global - Alias
----------------------------------
    alias.ci=commit
    alias.st=status
    alias.br=branch
    alias.co=checkout
    alias.df=diff
    alias.dc=diff --cached
    alias.lg=log -p
    alias.who=shortlog -s --
    alias.undo=reset --hard
    alias.new=!sh -c 'git log $1@{1}..$1@{0} $@'
    
3) Usefull command
----------------------------------
    git status 
    git add <file>

Show change

    git diff
    
Save code in memory

    git stash save "last changes" 

Get latest update

    git fetch origin

Get latest update and apply on given branch

    git pull origin MY_BRANCH_NAME
    
Create new branch 

    git checkout -b MY_BRANCH_NAME
    
Change branch name 

    git branch -m NEW_BRANCH_NAME  
    
Apply all stashed code in current branch

    git stash apply

Manage change 

    git commit -m "your descriptif here"
    git push origin MY_BRANCH_NAME
    
    
Remove branch

    git branch -d MY_BRANCH_NAME
    git branch -D ANOTHER_BRANCH_NAME
    
Get modification from a specific commit

    git cherry-pick COMMIT
