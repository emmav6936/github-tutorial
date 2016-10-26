# GitHub Tutorial

_by Emma Velazquez_

---
## Git vs. GitHub
Git is version control. As you work on your code you can commit changes, which is taking snapshots of your code, to see what you've done piece by piece. GitHub is an online server where you can use Git. It is a cloud where all your work is saved and you can use it from any device with internet access. You can also use GitHub to collaborate with other uses on projects. While GitHub requires Git, Git does not require GitHub.





---
## Initial Setup
To set up your GitHub account:   
* Go to **GitHub.com** and create an account  
    * _Sign In with a username and a password you'll remember (for example HSTAT Students could use their hstat.org account)_
* After you've signed up check your email to verify your GitHub account

To set up your Cloud9 account:
* Create an account on Cloud9 using your first and last name then create a username _(for example HSTAT students could use their HSTAT username)_
* Go to **c9.io** and in the top right corner there is a gear icon, click on it and go to **Connected Services**, connect to GitHub

To set up your SSH key:
* Go to GitHub and click on your profile icon in the top right corner
* Go to settings
* In the left sidebar click on SSH and GPG keys
    * click on New SSH key
* Give it a title _(for example Cloud9)_
* Go to Cloud9 and click on the gear icon 
    * click on SSH and GPG keys ->  New SSH key
---
## Repository Setup
A repository is  
To set up a repository use the command git init
If you mistakenly initialize git in the wrong directory use ```rm -rf .git``` to uninitialize

####  REMOTE
## Workflow & Commands
* ``` git add ``` - This adds your change(s) into the staging area. Do this before you do ``` git commit ```

