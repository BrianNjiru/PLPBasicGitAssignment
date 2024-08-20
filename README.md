# PLPBasicGitAssignment
Hands-On Assignment: Basic Git And GitHub Workflow
Objective:

The objective of this assignment is to familiarize students with the basic workflow of creating a GitHub repository, connecting it to a local folder, and making commits and pushes.

Steps followed:

#1.Github repository creation.


I logged into my Github account and created a repository named "PLPBasicGitAssignment".


#2.Local Setup.

 
I created a local folder named PlPAssignment and initialised a new git repository in it using `git init`. 

I then linked the github repository that was created in step one to the local repository using  `git remote add origin <repository-url>`, with "repository-url" being the current github repository.


#3.Making changes.


For this step I created a text file, `hello.txt`, in my local repository and made the changes viible in the github repository by pushing the changes.


#4.Comitting changes.

`git add hello.txt`
` git commit -m "Add hello.txt with a greeting"`


#5.Pushing to GitHub


Initially the `git push -o origin main` command failed, giving the following error;
`error: src refspec main does not match any
error: failed to push some refs to 'https://github.com/BrianNjiru/PLPBasicGitAssignment'`
After a quick google search, I changed the branch to `master`, as it was the branch I was currently using. I ran the command   `git pull --rebase origin main` which updated the github repository and then pushed the changes to the github repository using `git push -u origin master`.
