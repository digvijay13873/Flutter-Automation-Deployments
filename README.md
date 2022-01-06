Steps to Release apk using GitHub Actions

STEP 1:- Create Repository

 a. Login to your Github account
 b. In the upper-right corner of any page, use the drop-down 
 
 c. Type a name for your repository, and an optional description.
 
 d. Choose a repository visibility
.  
 e. Click Create repository.
 

STEP 2:- Pull Flutter code from your local machine

a.	Open Git Bash.
b.	Change the current working directory to your local project.
c.	Initialize the local directory as a Git repository.
            $ git init -b main
d.	Add the files in your new local repository. This stages them for the first commit.
     $ git add .
e.	Commit the files that you've staged in your local repository.
     $ git commit -m "First commit"

f.	At the top of your repository on GitHub.com's Quick Setup page, click to copy the remote repository URL. 
g.	In the Command prompt add the URL for remote repository where your local repository will be pushed.
     $ git remote add origin  <REMOTE_URL> 
# Sets the new remote URL
     $ git remote -v
# Verifies the new remote URL

h.	Push the changes in your local repository to GitHub.com.
    $ git push origin main

Note: - Always compile your code on Local Machine first before using Git Action
STEP 3:- Use Git Action
a.	 Check all the files that you have pushed to your github account
b.	 Go to Actions tab 
 
GitHub Actions uses YAML syntax to define the workflow. Each workflow is stored as a separate YAML file in your code repository, in a directory called .github/workflows.
c.	Setup your workflow by clicking the highlighted link or choose a suggested workflow for your repository. 
d.	Check the YAML script and Click the “Commit” button. 



STEP 4:- View Workflow Activity

a.	Once your workflow has started running, you can see a visualization graph of the run's progress and view each step's activity on GitHub.
b.	On GitHub.com, navigate to the main page of the repository.
c.	Under your repository name, click Actions
. 
d.	In the left sidebar, click the workflow you want to see.
 
e.	Under "Workflow runs", click the name of the run you want to see 
f.	View the results of each step. 
g.	Find APK
  
 
  Where to find the apk?
  
1.	 Go to your Repository
2.	Click the Actions tab
3.	Select the desired workflow
4.	Click on successful workflow
5.	Towards bottom of the page-->artifacts/release-apk

