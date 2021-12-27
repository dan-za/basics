# Linux Commands

| Command                       |           Description           |
|-------------------------------|:-------------------------------:|
| pwd                           |      Path of folder I'm in      |
| cd                            |        Change directory         |
| ls                            |    Show content of directory    |
| cat                           |        List file content        |
| touch <file>                  |          Create a file          |
| cp <target> <destination>     |           Copy files            |
| mv <target> <destination>     |      Move or rename files       |
| mkdir                         |     Create a new directory      |
| rm                            |   Remove files or directories   |
| locate (-i =ignore-case)      |      Locate a file by name      |
| find <directory> -name <name> |      Finds a file by name       |
| grep                          | Search for text in a given file |

## Show content of directory (ls)

| Command |             Description             |
|---------|:-----------------------------------:|
| ls -a   |          Show hidden files          |
| ls -al  | Also shows details like permissions |

## Concatenate (cat)

| Command                 |                    Description                     |
|-------------------------|:--------------------------------------------------:|
| cat > myFile            |                 Creates a new file                 |
| cat file1 file2 > file3 | Creates a new file with content of file1 and file2 |

## Remove (rm)

| Command           |         Description          |
|-------------------|:----------------------------:|
| rm -r <directory> | Remove directory and content |
| rm -i *           |  Prompt before file removal  |


# GIT Commands

| Command                    |                Description                |
|----------------------------|:-----------------------------------------:|
| git status                 |      State of git working directory       |
| git add -u .               |   Add deleted and unmodified files only   |
| git add (-A)               |             Add (all) file(s)             |
| git commit -m 'comment'    |       Commit changes to local repo        |
| git push origin master     | Push changes in local repo to remote repo |
| git checkout -b branchName |        Create and switch to branch        |