### SSH Clone Exercise

First, let us create a new Repository by name SecondRepo on the Server and initialize it with a README file <br>

![](images/SecondRepo.png?raw=true)
>Do not forget to choose the option - Initialize this Repo with a README

Once the Repository is created, you can find the URL (either HTTPS or SSH):

![](images/SecondRepoURL.png?raw=true)

Use Git Bash and navigate to any place-holder folder (not within any existing Git Repository) and type in :

```
# Let us use the SSH URL to clone this repository
git clone git@github.com:rchidana/SecondRepo.git
#If you use SSH URL, you are prompted for passphrase and if you use HTTPS URL, you will be prompted to enter your GitHub username (or registered email) & password
```

This will create a folder by name - SecondRepo - which is an exact replica of the Server Repository <br>
Please check remotes, commits and their timestamps <br>

Please peform some new code update, commit it and then push it to the server <br>