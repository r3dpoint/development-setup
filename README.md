# development-setup
scripts to setup development

# Requirements
- A GitHub Token: https://help.github.com/en/articles/creating-a-personal-access-token-for-the-command-line
- When prompted for GitHub credentials provide your GitHub username for username and your GitHub token for password

# Install
Download the script into your home forlder:
```
curl --remote-name https://raw.githubusercontent.com/r3dpoint/development-setup/master/development-install
```
Review the script (avoid running scripts you haven't read!):
```
less development-install
```
Execute the script:
```
sh development-install 2>&1 | tee ~/laptop.log
```
Optionally, review the log:
```
less ~/laptop.log
```
## Debugging
Your last Laptop run will be saved to `~/laptop.log`. Read through it to see if you can debug the issue yourself. If not, copy the lines where the script failed into a new GitHub Issue for us. Or, attach the whole log file as an attachment.
## What it installs
- Homebrew (and XCode Command Line tools, which include Git)
- Heroku
- nvm
- rbenv
- postgres
