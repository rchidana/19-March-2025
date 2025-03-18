### To create a new Repository called - FirstRepo - from client (Git Bash) and then push it to the server

```sh
$ mkdir FirstRepo
$ cd FirstRepo
$ git init   #This will create the magical .git folder in this directory
```
>From now on, Git will track any changes (files added, modified and/or deleted) that occur in this folder

Create, add or edit files in this folder and when you have completed the changes

```sh
$ git add .
$ git commit -m "My first changes" #Any meaningful message of your choice
```
>You can keep making changes to the repository contents and commit as many changes as you want.

Once you are done with your changes, you would want to push this Repository on to the server and for this, you would need to create a skeleton of your Repository on the server and the name of the Repository on the server should match the Git Bash directory that you have created (FirstRepo in this case).

Go ahead & Create a Repository on the Server, make it a Public Repository and DO NOT choose - 'Initialize with a README'
![](images/FirstRepo.png?raw=true)

GitHub displays the set of commands required to push contents from the Git Bash prompt and you would notice that it provides specific commands for HTTPS & SSH:
![](images/FirstRepoURL.png?raw=true)

Since we only have HTTPS authentication enabled, let us use HTTPS URL <br>

Modify the branch name (if need be) and then run the push command from command prompt <br>

Check on GitHub Server if your repository is available, check on code commits, timestamps etc <br>