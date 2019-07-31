# Git Flow Command Line Tool 101

## Overview
The Git Flow Command Line tool helps you manage your Git Flow process with stream lined commands. The commands are a wrapper around the traditonal git commands. In this document we will go over some of the commands that run behind the scenes when you are using the git flow command line tools.

*Disclaimer - the git flow command line tool is not a replacement for git, it is just a wrapper around git commands. This is an optional tool to use. Its mainpurpose is to help you with the git flow workflow and to not have to memorize a bunch of git commands in order to achieve that workflow. Also, I have not seen a way to use this with any git GUI tools.*



## Git Flow Workflow Overview
Gitflow Workflow is a Git workflow design that was first published and made popular by Vincent Driessen at nvie. The Gitflow Workflow defines a strict branching model designed around the project release.  

Gitflow is ideally suited for projects that have a scheduled release cycle. It assigns very specific roles to different branches and defines how and when they should interact. In addition to feature branches, it uses individual branches for preparing, maintaining, and recording releases.Y ou get to leverage pull requests, isolated experiments, and more efficient collaboration.

Full overview [HERE](https://www.atlassian.com/git/tutorials/comparing-workflows/gitflow-workflow)

## Common git flow commands mapped to git commands
### Initilaze
* When initizaling a project with the git flow commands the first command we need to run is :
```
git flow init
```
Git equivalent commands
```
git init
git commit --allow-empty -m "Initial commit"
git checkout -b develop master
```
#### What it looks like
![img](img/git_flow_init.png)

### Features
* When we pick up a story and want to start a feature we will need to enter this command :
```
git flow feature start MYNEWFEATURE
```
Git equivalent commands
```
git checkout -b feature/MYFNEWEATURE develop
```
#### What it looks like
![img](img/git_flow_feature_start.png)

