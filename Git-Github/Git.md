# Git Commands

## Configuration:

- git config --global user.name "Nome Sobrenome"
- git config --global user.email "email@gmail.com"
- git config --golbal core.editor vscode 

## Consulting: 

- git config --list
- git config user.name
- git config user.email
- git config core.editor

## Commands:

- git init ->                                creates a new repository
- git add <file> ->                          adds a <file> to the staging area
- git add -A, git add . ->                   adds all files to the staging area
- git log ->                                 shows the history of all the commits
- git restore <file> ->                      goes back to the last commit and erase all modifications made after that
    
- git reset --soft  <id.commit> ->           goes back to a specific commit
- git reset --mixed ->                       ...cleaning the staging area
- git reset --hard ->                        ...and reversing all the modifications made in the machine 

- git commit -m "message" ->                 the changes made that are in the staging area are saved in the git repository
- git status ->                              shows the current state of the Git working directory and staging area

- git branch ->                              shows all the branches in the directory
- git branch -M <branch.name> ->             "renames" the branch to <branch.name>
- git branch <branch.name> ->                creates a new branch called <branch.name>
- git branch -D <branch.name> ->             deletes the <branch.name>
- git checkout <branch.name> ->              navigates to <branch.name>

- git checkout HEAD <file> ->                replaces the <file> with the last commited version of it 

- git diff ->                                shows all the modifications made
- git diff --name-only ->                    shows only the names of all the files that were modificated

- git remote add origin <remote repo url> -> creates a connection to the remote repository wich is being named origin(can be named differently. Ex: git remote add agustin <remote repo url>)
   
- git push origin <branch.name> ->           sends the <branch.name> to the remote repository
- git push origin :<branch.name> ->          removes the <branch.name> from the remote repository

- git pull origin <branch.name> ->           pulls the files from the remote repository(origin) to the local repository

- git clone <URL> ->                         clones a repository using the URL of the project
