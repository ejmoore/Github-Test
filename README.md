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
