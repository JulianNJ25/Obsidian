# Shell: 
Command Interpreter that allows to execute operations using text and commands. The foundation for running **scripts**

Some of the more popular shells include: Bash, Csh, Zsh, and Fish

# Most Common Commands

## man
**man**ual, its a command we can match with any other command so we can know what they do and how they work -> `man <command>`

Example: `man ls`

However, man pages even though are super useful they can be WAY too detailed, if we'd like to get **shorter information** we can install **tldr**, a community tool meant to simplify man pages

Example: `tldr ls`

## ls
**l**i**s**t all the files and folders inside a folder
We can specify if we want to see the contents of an specific folder

Example: `ls /bin` -> will display all the files inside the /bin folder

'ls' can be combined with a multitude of **flags** that expand on the functionality of ls, like `ls -a`-> will print all files included hidden files (plain ls does not do that)

## cd
**C**hange **D**irectory, we can move into a folder with this command 
`cd fruits` -> entering fruits folder

we can also go back to the parent folder with **..** this key character basically means "current folder"
`cd ..` -> back to the home folder (or folder containing fruits folder)

we can also browse folders in a variety of ways by combining .. and folder paths
`mkdir fruits`
`mkdir vegetables`
`cd fruits`
`cd ../vegetables` -> goes back to parent folder and then enter vegetables folder

However for the moment those are relative paths for more accurate results we can use absolute paths.
An **absolute path** will always start from the **root** folder -> `/`
`cd /etc`

## pwd
prints the current folder path, this is useful in situations on where we are lost and want to know in which path we currently are

## mkdir
'**M**a**k**es a **dir**ectory' or we can say it creates a new folder as well
`mkdir dog`

We can create multiple folders all at once
`mkdir dog parrot`

We can create nested folders by adding the `-p` option
`mkdtir -p pet/dog`



