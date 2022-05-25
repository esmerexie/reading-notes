# [Git intro](https://blog.udemy.com/git-tutorial-a-comprehensive-guide/)

>It is important to note that when dealing with [Git](https://blog.udemy.com/git-tutorial-a-comprehensive-guide/), you must have a basic understanding of your computer's terminal. 

## History of Version Control

The history of files managed by programmers in short went like this. 

1. **LVC (Local Version Control)** - Was when programmers didn't have the ability to store and distribute files on the cloud but rather had to do it locally on one server's hard drive.

2. **Centralized Version Control systems (CVCS)** - Over time programmers wanted collaboration with a team on a single file or files. So this led to Centralized version control. This gave them the ability to programmers to access the files and all changes and versions would be stored in one system.

3. **Distributed Version Control systems (DVCS)** - One major flaw of the CVS or Centralized version control was the single point of failure. Meaning that if the server were to shut down, all accessibility to the file was gone. This led to the *Distributed Version Control*. This allowed progammers to mirror the files or repositories of the original file meaning that if one were to lose it, another person would still have the file.

## Git 
- is a DVCS
- can relies on local operations. Meaning it doesn't need to be worked on online. 
- tracks changes
- **greatly** minimizes the possibility of irreversible damage to the files.

### Git Terminal Commands :

These are some of the basic git terminal commands.

This line is used to check settings in your terminal.

> git config --list

This line is used to clone the repository off of GetHub

> git clone (Your URL here)

This line is used to check the file status

> git status

To add a file 
> git add (file name)

or All files

> git add .

When committing a file us this command plus a message detailing the commit

> git commit -m "your message here"

When Committing all changes 
> git commit -a

When pushing changes to the main file. 

> git push origin master

# For more on learning the intro to Git click [Here](https://blog.udemy.com/git-tutorial-a-comprehensive-guide/)

