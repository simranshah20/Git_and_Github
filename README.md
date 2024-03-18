In this repo I have learnt about Git and Gihub.
Here is few commands which help me to understand the basics concepts of git:

1. git --version => This command will show you the version of your installed git in your system.
2. git config --global user.name "my name" => This command sets up a default username globally
3. git config --global user.email "your email" => This command sets up a default email id globally
4. git config --list => This command list all the configurations that are set up globally
5. git clone <repo url> => This command downloads or clones the repository from given url into local machine(laptop,pc).
6. git status => This command shows the state of files in the directory i.e., untracked, modified or staged. It also lists any changes that haven’ or for specific project.
7. cd => It changes the current working directory to another directory.
8. ls => Lists out the contents of the current folder/directory.
9. pwd => Prints the full path of the current working directory.
10. ls -a => This command lists out all the hidden files.
11. git init => Initializes a new git repository inside the current
12. git add <-file name-> => Adds the file(s) to staging area so that it can be committed.
    13.git add . => This command add all the untracked files present in the current directory to the staging area.
13. git commit -m "some message" => Commits the added file(s) with a specific message.
14. git remote add origin <url> => Connects your local repository with a remote one (Github). Here url would be
15. git log => Displays the history of commits made.
16. git remote -v => This command shows the url of the remote repository where our local repository is connected to.
17. git push origin main => This command transfers (pushes) the changes from local repository(laptop,pc) to remote repository(github).
    Here origin refers to remote repository from where we clone our project.

To push my local code to GitHub

1. First, I need to make sure that I am logged into GitHub on my machine using the below command :
   sh$ gh auth login

2. Then I should connect my local
   repository to the GitHub repository by doing following steps:
   sh$ git remote add origin https://github.com/<username>/<repo>.git
   (Replace <username> with yours Github UserName & <repo> with Your Repo Name.) 3. After connecting your local repository to the GitHub repository, use the following command to push your code to the remote repository:

3. check status of connection by typing :
   sh$ git remote -v

4. now add the files to the staging area (using wild card \* means adding all files):
   sh$ git add .

5. Now commit those changes with a meaningful message :
   sh$ git commit -m "Initial commit."

6. Push the changes to the connected GitHub repository:
   sh$ git push -u origin main or git push -u origin main
