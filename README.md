cd Desktop -->cd = "change directory"

-->This command moves you into the Desktop folder.
mkdir git-tutorial -->"make directory"
-->This creates a new folder called git-tutorial on your Desktop.
cd git-tutorial/-->Moves you into the new git-tutorial directory you just created.
code .-->Opens the current folder (. means current directory) in Visual Studio Code.
git init -->Initializes an empty Git repository in the current folder.Creates a hidden .git folder where Git tracks changes.
git status-->Shows the current state of your Git repo.Tells you things like:Which files are being tracked or not.If there are any changes to be committed.If you're on a branch, etc.
git add -->What it does:Moves changes (new or modified files) into the staging area.You're basically saying: "Hey Git, I'm planning to include these changes in my next commit."
git add . -->OR to add everything that’s changed.The . means "add all changes in the current folder and below."
git commit -m "" -->Takes everything in the staging area and saves it as a snapshot in Git history.Requires a message describing what you did.



                Full Example Workflow:
touch index.html           # Create a new file
git status                 # Shows the untracked file
git add index.html         # Stages the file
git status                 # Shows it's staged for commit
git commit -m "Create initial index.html"  # Commits it
git rm --cached <filename>          #Removes a file from Git staging and tracking, but keeps it on your computer.

You need to tell Git your name and email — this info gets added to each commit you make (but doesn't log you into GitHub).
Set it globally (for all future repos):
git config --global user.name "Your Name"
git config --global user.email "your@email.com"

Full Example Workflow:
git config --global user.name "Your Name"
git config --global user.email "your@email.com"
git init
git add .
git commit -m ""
git remote add origin https://github.com/Aldrinnnnnnnnnnnnnn/HTML-2025.git
git push -u origin master

You modified in your code and you want to add and commmit to repo
1.git add . && git commit -m "Comment"


