# GitHub Tutorial

_by Emma Velazquez_

---
## Git vs. GitHub

![](https://preview.c9users.io/emmav6936/github-learning/github-tutorial/Screen%20Shot%202016-10-26%20at%208.43.27%20AM.png?_c9_id=livepreview0&_c9_host=https://ide.c9.io)
Git is version control. As you work on your code you can commit changes, which is taking snapshots of your code, to see what you've done piece by piece. GitHub is an online server where you can use Git. It is a cloud where all your work is saved and you can use it from any device with internet access. You can also use GitHub to collaborate with other uses on projects. While GitHub requires Git, Git does not require GitHub.




---
## Initial Setup
To set up your GitHub account:   
* Go to [**GitHub.com**](https://github.com/) and create an account  
    * _Sign In with a username and a password you'll remember (for example HSTAT Students could use their hstat.org account)_
* After you've signed up check your email to verify your GitHub account

To set up your Cloud9 account:
* Create an account on Cloud9 using your first and last name then create a username _(for example HSTAT students could use their HSTAT username)_
* Go to [**c9.io**](https://c9.io/) and in the top right corner there is a gear icon, click on it and go to **Connected Services**, connect to GitHub

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
A repository on Cloud9 is where you store the work you do using git.
To make a directory use the command ```mkdir <repo-name>```
To turn a directory into a repository use the command ```git init```  
If you mistakenly initialize git in the wrong directory use ```rm -rf .git``` to uninitialize.

#####  REMOTE

A remote repository is where your work is stored on the cloud. _GitHub is an example of a remote repository platform_

Your local repository (_Cloud9_) and your remote repository (_GitHub_) should be linked so that you are able to push (_send/upload/export_) to the cloud and pull (_download/import_) from it.

To do this you need to:
*Go to GitHub and in the top right corner you should see a plus sign icon, click on it
* Make a new repo _**IT MUST HAVE THE SAME EXACT NAME AS YOUR CLOUD9 REPOSITORY**_
* Create repository

##### ADDING AND COMMITING
![](https://preview.c9users.io/emmav6936/github-learning/github-tutorial/Screen%20Shot%202016-10-26%20at%2012.43.19%20PM.png?_c9_id=livepreview3&_c9_host=https://ide.c9.io)
A commit is similar to saving your progress in a video game. When you commit you save everything that you've staged. To commit you mush first add your work to the staging area. You do this with the command ```git add``` for example if I were to stage this README I would use the command ```git add README.md```
A helpful command is ```git status``` especially for when you are committing something. Git status will tell you what you've staged in the command line in green text and new work will be in red text.

Once you've added everything to the stage now you can commit you use the command   
```git commit -m "<YOUR COMMIT MESSAGE HERE>"```  
NOTE: You're commit message should be clear and concise so that you know what the commit does

## Workflow & Commands
* ``` git add ``` - This adds your change(s) into the staging area. Do this before you do ``` git commit ```

