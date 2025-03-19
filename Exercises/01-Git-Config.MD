# Git Initial Configuration

Before begining any Git Operations from the Client, you would need to configure the Username & Email ID of the Developer who is performing Git Operations. Open up the Git Bash command and key in your Username & Email ID: <br>

```
git config --global user.name "John Doe"  #Double Quote required
git config --global user.email johndoe@example.com     #No double quote for email ID
#Check if the settings got picked up correctly
git config --list

```

>If your details (username & email ID) are not picked up correctly, do not fret, check if the commands were entered correctly and repeat them any number of times till you get it correctly

Configurations are stored at various levels - System Wide, Global & Local (Repo specific) <br>
One can manually edit the settings by opening up respective conf files <br>
Easier way is to use config command to unset or update value <br>

```
git config --help

# Let us unset a global setting "user.name"
git config --global --unset user.name
# We can now give a different value for this configuration
git config --global user.name "Anand R"

# Or we can try to overwrite the setting with one command
git config --global user.name "Anand R"

# Check if our new values have been picked up by git
git config --list

```

Git client configurations persist in file(s) by name .gitconfig/gitconfig and are stored at various locations in the local machine <br>

```
# Let us check the origin of the configurations that are currently used
git config --list --show-origin

```











### GitHub Cheat-Sheet Complete Reference --> https://github.com/rchidana/Git_Cheat_Sheet