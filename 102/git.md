# Reading notes for Git Intro- Revisions to the Cloud

## Version Control

- Allows you to revisit various versions of a file
- gives abilility to revert a file or project to a previous version and compare changes.
- allows mistakes to easily be repared

1. Local Version Contol- entails one database to store changes to files
2. Centralized Version Control (CVS)- Allows for collaboration within dev team on a single file
3. Distributed Version Control (DVCS)- Allows to creat mirrored repositories. Helps to replace lost information. Also allows multiple people to collaborate with each other on a joint project. Simultaneous workflows

## What is Git

- Snapshots
  - Git is a DVCS that stores data in a file system made up of snap shots
  - Each time you save Git creates snapshot
- Local Opperations
  - Relies on local operations
- Tracking Changes
- Loss of data
- States- 3 main- committed, modified and staged
  - Committed Data is securely stored in a local database
  - Modified - File has been changed but not committed to the database
  - Staged - Flagged a file's changed versions to be committed in the next snapshot
- Graphical Clients- Git has inherent Graphical User Interface (GUI) tools - You can also utilize 3rd party tools
  - Other GUI clients can be accessed through [GUI Clients](https://git-scm.com/downloads/guis)

## Initial Customization

- Configuration of Variables- (git config) allows the setting of configuration variables
- Identity Setting -
      - fit config --global user.name "Jane Smilth"
      - fit config --global user.name "exampel@email.com"  
   -confirm
      - git config -- global user.name (render name)
      - git config -- user.email (render email)

## Check settings

- git config --list

## Get help

- git help command
- git command --help
- man git-command

## Importing

   1. cd test
   2. git init
   3. git add *.c
      git add LICENSE
      git commit -m "any message here"

## Cloning

- to create copy of existing Git use - git clone URL
- this copies all version and files of a project
- retrieves for editing - a copy of the newest version of the project

## Local Repository Structure - 3 Components

1. Working Directory: The actual files Reside here
2. Index: The area used for staging
3. Head: Points to the most recent commit

## Saving Changes - all files in tracked or untracked state

- Tracked - Files can be modified, unmodified, or staged; they were part of the most recent file snapshot
- Untracked -  were not in the last snapshot and do not currently reside in the staging area.

## Check File Status

- use - **grit status**

## Tracking and Staging new file

- Single file **git add file name**
- All Files **git add .**

## Committing a File

- **git commit -a**

## Push Changes

- **git push origin master**

## Stashing Changes

- When not ready to commit to changes use **git stash**
- When ready to commit changes use **git stash apply**

## Cloned Repositories

Git will automatically give the name "origin" to the server from which you cloned and named master

[<back](README.md)
