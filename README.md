# technicalwriting
Notes and insights I've gained from my technical writing training

Git is a version control system; GitHub is a commercial platform that lets you host files remotely through Git.

# Docs Like Code
Writing docu the same way you treat writing code.

Can mean three things
1. Docu in text format, not binary (meaning you can open in a text editor)
2. Includes use of version control tools like Git
3. You use a review process similar to code reviews 

**XML** (eXtensible Markup Language) is a combo of text/tags. Works well for DITA, but not Docs Like Code.

**Markdown** is a simple markup language with no tags (< >). It has many variations ("flavors") and works well with Docs Like Code.

**reStructured Text** is a little more complex than Markdown, but you can extend its functionality. This works well for Docs Like Code.

**AsciiDoc** similar to reStructured Text.

GitBook is a tool made specifically for generating docu using Git.

# Version Control
As you write and rewrite docu, you create new versions. It's important to keep old versions, but manually keeping track is a hassle.

In version control, multiple users manage those versions as if they all had the same name. Can help manage multiple people working on the same doc from different locations.

Instead of storing every version of a file, it stores the differences between versions, so it takes up less space.

## Git Innovations
Git manipulates using the file system, so file content changes with git commands.

Separates commit and push, so marking a file stays local until you are ready to commit, or upload.

Still, need a commercial platform for ease of use. GitHub is popular choice, but also Bitbucket, GitLab, and Beanstalk.

# Getting Started with Git
Contains a command line and a GUI (or Graphical User Interface)

Command line gives you full power, and is not much less confusing than GUI. Most people end up using command line anyway, so this course uses it anyway.

Text editors are recommended for Git. Macs usually come with Git in the form of Terminal.

# Getting Started with GitHub
A way to host content remotely and allow other users to read/write versions

A repository (or repo) holds a directory structure (so folders) with files. They contain not just current versions, but old versions, too. Exist both remotely and locally.

You can create a repo in Git, then "push" to GitHub, but it's easier to create in GH, then "clone" it locally. To clone, you need the README file, which is basically the docu for the repo.

Once a repo is created, GitHub shows you its path in the Code button.

# Command Line
This course uses Unix commands:
* **pwd** (print working directory) tells you what folder you are in
* **ls** (list) tells you what files are in current folder
* **cd** (change directory) moves you to a new folder; type .. for one directory up and ~ to go to home directory
* **mkdir** (make directory) creates a new folder

## Command Line Shortcuts
* **Tab** fills in the rest of the name.
* **Up arrow** repeats previous command
* **Several up arrows** go through history of commands
* **Down arrow** goes forward in command line history

## Example git commands
* git config --list
* git config --global user.name "Peter Jurich"
* git commit -m "Marketing changes"

# Git Concepts
As you work with files in Git, they go through four stages
1. **Unstaged**: You've made a local change to a file (including added/deleted a file). You've made a change you're not sure you want to keep.
2. **Staged**: You've marked a local change as something you'd like to commit and save in Git. You're pretty sure you'd like to keep the change. Use `git add` command.
3. **Commit**: You have saved the file in Git. Each commit has a description to help you remember what changed. You definitely want to keep the change. `git commit`
4. **Pushed**: File has been uploaded to Git server (or GitHub) for others to access. You'd like others to see the changes. `git push`

Git treats text and binary (images, audio, video) files the same.

# Adding files to a repository
## Useful git commands
`git status`: provides useful info
`git add`: moves one or more files from unstaged to staged
`git commit`:commits any staged files
`git push`: uploads committed files to GH
