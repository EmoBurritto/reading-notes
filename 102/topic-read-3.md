# Git Intro

## Version Control

**Local Version Control**

*Consits of one database on a hard disk to store file changes*

**Centralized Version Control**

*Allows multiple contributors to add to file. However, there is still one single server but allows a team to divy up the work and see what others have worked on. Still prone to corruption and losing all datat except what's on local files.*

**Distributed Version Control**

*By allowing mirroring repositories for contributers, CVS corruption is taken out tof the equation. Git is a DVCS.*

## Git Componets

*Snapshots are used by the git commit command allowing storing of files with a refrence to the identical version only. Git is local only, no need to be online. Git tracks file corruption and loss of information in transit when changes are applied. Extremely hard to lose data or file to be corrupted when snapshot taken. Three main states of files in Git:*

- Committed (file secured)
- Modified (file change but not secured)
- Staged (file changed and committed for next snapshot)

## Graphical Client 

*Third Party tool or Graphical User Interface(GUI) can be used to make Git easier.*

## Initial Customization

*Use command ***git config*** to see settings of terminal. You can apply user name and password to stay online with Git terminal for future use.*

## Git Help 

*Use command ***--help*** to pull up a glossary for help in looking for a common command.*

## Importing

*Use command ***git init*** to import selected file; _cd file name_*

## ACP
*ACP(Add, Commit, Push) is used to permamently add a chnage into a file after changes or revisions have been made. The commands for ACP are:
- ***git add file name***
- ***git commit -m "insert why you made changes"***
- ***git push origin master***

*However, if not ready to make permanent changes use command ***git stash and git git stash apply*** to temporarily hide and retrieve set changes*

#### My Github profile lives here [github.com/JoseGonzalez1394](https://github.com/JoseGonzalez1394)

![](/WIN_20220627_05_31_26_Pro.jpg)
