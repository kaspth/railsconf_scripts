# RailsConf Scripts

This repo includes scripts for pracitcing the tools we will learn at RailsConf.

First clone the repo, then install the cached gems:

```
cd railsconf_scripts

# if using windows
git checkout windows
bundle install --local

# if using mac/linux stay on msater
bundle install --local
```

RailsConf talk description:

> **Breaking Down the Barrier: Demystifying Contributing to Rails**

> Contributing to Rails for the first time can be terrifying. In this lab I’ll
make contributing to Rails more approachable by going over the contributing
guidelines and technical details you need to know. We’ll walk through traversing
the source code with tools such as CTags, source_location and TracePoint.
Additionally, we’ll create reproduction scripts for reporting issues and learn
advanced git commands like bisect and squash. At the end of this session you’ll
have the confidence to fix bugs and add features to Ruby on Rails.


## Executable Scripts

In this repo there are Active Record executable scripts and a couple Ruby scripts
for my lab at RailsConf 2015 on Contributing to Rails.

### Running the scripts

To run:

```
cd railsconf_git/
bundle exec ruby ar_script_name.rb
```

## Practicing Git

Checkout the `practicing-git` branch.

The `practicing-git` branch is a branch for practicing git commands for my RailsConf
lab on contributing to Rails. Please see that branch for git the git commands.

### Interactive Rebase

`git rebase -i master`

### Undoing Mistakes in Git

#### Reset

`git reset --hard ref`

`git reset --soft HEAD~N`

`git reset --soft HEAD@{1}`

#### Reflog

`git reflog`

### Using Git to Find Where Code was Introduced

#### Bisect

`git bisect start`
`git bisect bad`
`git bisect good ref`
`git bisect reset`
