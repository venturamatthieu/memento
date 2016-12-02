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

