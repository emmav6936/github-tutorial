# GitHub Tutorial

_by Emma Velazquez_

---
## Git vs. GitHub

![](https://preview.c9users.io/emmav6936/github-learning/github-tutorial/Octocat.png?_c9_id=livepreview0&_c9_host=https://ide.c9.io)

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
![](https://preview.c9users.io/emmav6936/github-learning/github-tutorial/remote%20repository%20image.png?_c9_id=livepreview2&_c9_host=https://ide.c9.io)
A remote repository is where your work is stored on the cloud. _GitHub is an example of a remote repository platform_

Your local repository (_Cloud9_) and your remote repository (_GitHub_) should be linked so that you are able to push (_send/upload/export_) to the cloud and pull (_download/import_) from.

To do this you need to:  
* Go to GitHub and in the top right corner you should see a plus sign icon ![](https://preview.c9users.io/emmav6936/github-learning/github-tutorial/plus%20icon.png?_c9_id=livepreview4&_c9_host=https://ide.c9.io), click on it
* Make a new repository _**IT MUST HAVE THE SAME EXACT NAME AS YOUR CLOUD9 REPOSITORY**_ ![](https://preview.c9users.io/emmav6936/github-learning/github-tutorial/create%20a%20new%20repo.png?_c9_id=livepreview7&_c9_host=https://ide.c9.io)
* Create repository
* In quick setup make sure you are using an SSH Key which is more efficient than a HTTPS Key because you don't have to put your username and password in everytime you need to push

###### Important Commands to use when setting up your remote repository

* ```git remote add <name> <url> ``` for example ```git remote add origin git@github.com:emmav6936/model-repository.git ```
* ```git push -u <name> master``` for example ```git push -u origin master``` 

These commands link your local and your remote and you only need to do this once per repository 

###### To completely remove a repository:
* On Cloud9: ```rm -rf <your repo name>``` for example ```rm -rf model-repo```
* On GitHub: 
    * Go to settings and scroll down to the **Danger Zone** ![](https://preview.c9users.io/emmav6936/github-learning/github-tutorial/danger%20zone.png?_c9_id=livepreview5&_c9_host=https://ide.c9.io)
    * Click on **Delete this Repository**
    * A box will pop up saying _Are you ABSOLUTELY sure?_ Type in the name of your repository ![](https://preview.c9users.io/emmav6936/github-learning/github-tutorial/are%20you%20absolutely%20sure.png?_c9_id=livepreview6&_c9_host=https://ide.c9.io)

##### ADDING AND COMMITING
![](https://preview.c9users.io/emmav6936/github-learning/github-tutorial/Screen%20Shot%202016-10-27%20at%2011.27.47%20AM.png?_c9_id=livepreview1&_c9_host=https://ide.c9.io)
A commit is similar to saving your progress in a video game. When you commit you save everything that you've staged. To commit you mush first add your work to the staging area. You do this with the command ```git add``` for example if I were to stage this README I would use the command ```git add README.md```
A helpful command is ```git status``` especially for when you are committing something. Git status will tell you what you've staged in the command line in green text and new work will be in red text.

Once you've added everything to the stage now you can commit you use the command   
```git commit -m "<YOUR COMMIT MESSAGE HERE>"```  
NOTE: You're commit message should be clear and concise so that you know what the commit does

![](https://preview.c9users.io/emmav6936/github-learning/github-tutorial/Screen%20Shot%202016-10-27%20at%207.51.21%20AM.png?_c9_id=livepreview8&_c9_host=https://ide.c9.io)

## Workflow & Commands

Command | Definition
---------|------------
```mkdir <directory name>``` |make a directory
```cd <directory> ```| go into your directory
``` git init``` |initialize git/ turn your directory into a repository
``` rm -rf .git``` | unintialize git 
``` git add <file>``` |add to the stage
``` git commit -m "<commit message>"``` |take snapshot of code/save the version
```git log``` |see your past commits
 ```git status``` |see your changes
 ```git add remote origin URL``` |setup remote 
 ``` git push -u origin master```| setup remote (both of these are necessary)
 ```git push``` |export to the cloud
 ```git remote -v``` |see if your push worked
 ``` git clone``` | copies the entire repository

## Social Coding
 * fork & `clone`, pull requests and `pull`  
To fork is to take someone's work pull it down into your local repository and add to it, change it.
To do this you:
* Go to GitHub and onto the profile of the person whose repository you wish to fork 
* Click on their repository and in the top right there should be an icon that says fork ![](https://preview.c9users.io/emmav6936/github-learning/github-tutorial/Screen%20Shot%202016-10-27%20at%201.07.32%20PM.png?_c9_id=livepreview0&_c9_host=https://ide.c9.io)
* click _Clone or Download_ ![](https://preview.c9users.io/emmav6936/github-learning/github-tutorial/Screen%20Shot%202016-10-27%20at%201.07.46%20PM.png?_c9_id=livepreview2&_c9_host=https://ide.c9.io)
* Copy the URL ![](https://preview.c9users.io/emmav6936/github-learning/github-tutorial/Screen%20Shot%202016-10-27%20at%201.07.58%20PM.png?_c9_id=livepreview3&_c9_host=https://ide.c9.io)
* On Cloud9 use ```git clone <URL>``` 
* Make changes and requests 
* Save, add, commit, and push your changes to the cloud
* make a pull request ![](https://preview.c9users.io/emmav6936/github-learning/github-tutorial/pull%20request%20icon.PNG?_c9_id=livepreview0&_c9_host=https://ide.c9.io)

![](https://preview.c9users.io/emmav6936/github-learning/github-tutorial/fork%20and%20clone.png?_c9_id=livepreview3&_c9_host=https://ide.c9.io)