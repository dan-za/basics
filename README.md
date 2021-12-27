# Linux Commands

| Command                                       |                                Description                                 |
|-----------------------------------------------|:--------------------------------------------------------------------------:|
| pwd                                           |                           Path of folder I'm in                            |
| cd                                            |                              Change directory                              |
| ls                                            |                         Show content of directory                          |
| cat                                           |                             List file content                              |
| less                                          |                   List file content. Scrolling possible                    |
| touch <file>                                  |                               Create a file                                |
| ln -s <target> <link>                         |                         Create a symlink to a file                         |
| cp <target> <destination>                     |                                 Copy files                                 |
| mv <target> <destination>                     |                            Move or rename files                            |
| mkdir                                         |                           Create a new directory                           |
| rm                                            |                        Remove files or directories                         |
| locate (-i =ignore-case)                      |                           Locate a file by name                            |
| find <directory> -name <name>                 |                            Finds a file by name                            |
| grep                                          |                      Search for text in a given file                       |
| df                                            |                           Show disk space usage                            |
| du -h fileName                                |                               Show file size                               |
| head -n 10 fileName                           |                        Show first n lines of a file                        |
| tail -n fileName                              |                        Show last n lines of a file                         |
| diff file1 file2                              |                           Show diff of two files                           |
| chmod                                         |                          Change file permissions                           |
| chown                                         |                           Change owner of a file                           |
| top                                           |                           Show running processes                           |
| ctrl + r                                      |                    Reverse search for executed commands                    |
| wget <url>                                    |                               Download files                               |
| alias anExample='date +%H:%M:%S'              |           Create an alias. (Will be removed if shell is closed!)           |
| unalias anExample                             |                                Remove alias                                |
| let                                           |                      Evaluate arithmetic expressions                       |
| \>                                            |                           Overwrite file content                           |
| \>>                                           |                            Append file content                             |
| find /var -name syslog 2> /dev/null 1> syslog | Errors (2) will be removed. Only normal output (1) will be written to file |
| cmd1&#124;cmd2                                |                 Data from cm1 will be transferred to cmd2                  |
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

## File permissions (chmod)

``chmod u=rwx,g=rx,o=r fileName``

   - user can read, write and execute the file
   - group members can read and execute the file
   - others can read the file 

Alternative
``chmod 754 fileName``
   - 4 = read
   - 2 = write
   - 1 = execute
   - 0 = no permission
   - 7 = 4+2+1 (read, write, execute)
   - 5 = 4+1 (read, execute)


# GIT Commands

| Command                                                         |                          Description                           |
|-----------------------------------------------------------------|:--------------------------------------------------------------:|
| git init                                                        | Create an empty Git repository or reinitialize an existing one |
| git remote add origin git@github.com:dan-za/myRepo.git          |                     Add remote repository                      |
| git config --get remote.origin.url OR git remote get-url origin |                   Show remote repository URL                   |
| git status                                                      |                 State of git working directory                 |
| git fetch                                                       |                Checks if changes are available                 |
| git pull                                                        |                         Pulls changes                          |
| git add -u .                                                    |             Add deleted and unmodified files only              |
| git add (-A)                                                    |                       Add (all) file(s)                        |
| git commit -m 'comment'                                         |                  Commit changes to local repo                  |
| git push origin master                                          |           Push changes in local repo to remote repo            |
| git checkout -b branchName                                      |                  Create and switch to branch                   |
| git checkout master                                             |                         Switch branch                          |
| git merge branchName                                            |                Merge branch into current branch                |
| git branch -d branchName                                        |                      Delete local branch                       |
| git push origin --delete branchName                             |                      Delete remote branch                      |