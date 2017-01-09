STEP 1 : Create a new Repository

Log into github, and follow the instructions to create your repository

After your repository is created, create a directory on your local computer
	"cd ~"
	"mkdir HGD"

Set up that repository as a git repository
	"git init"

Create your first file for the repository and tell git to track it (README)
	"vim README.md" (Type your game idea here)
	"git add README.md"
	
Commit your changes to the repository
	"git commit -m "first commit""

Push your code to GitHub (First time only)
	"git remote add origin https://github.com/ejmoore/Github-Test.git"
	"git push -u origin master"

That's the basic setup! Now you can add files, commit and push things to your repository much more easily. As a general summary, you just told your computer that a directory is a git repository. You then created a file and told git to track it by adding it. You can then commit your changes including a short message covering what you've done for that commit. Finally you told git where it should push that commit to and then pushed it. Keep in mind that pushing will upload all of your committed code to your GitHub repository. You should commit code very frequently to avoid problems down the line.

In Review:
	Add a new file "git add filename"
	Commit your changes "git commit -m "message""
	push your code "git push" (Note that you no longer nead the "-u origin master")

STEP 2 : Branches

Branches are a way to organize your GitHub repository. They are absolutely essential to make sure you aren't stepping on anyone elses toes during development. Typically there will be a branch for each feature you are adding to your project. You can keep working on that feature until it's complete then you merge the branch back into the main project. Think of it like one giant commit for the entire feature.

To create a new branch it's another simple command
	"git checkout -b branch_name (this creates a new branch and switches to it locally)

To upload this branch to GitHub all you have to do is to push it
	"git push origin branch_name

There's one more thing you have to do before you can push any changes to your branch. On your first push after creating the branch type this instead
	"git push --set-upstream branch_name

Now you can work on you branch in the same manner as you were working on your project before by adding, commiting, and pushing. The key difference now is that as long as you're the only one working on your branch, all the settings, code changes, and additions implemented on this branch will only be seen while using this branch. This helps us avoid merge conflicts for simple things like changing variable values for testing purposes or adding a new method to a major class.


Test commit/push
