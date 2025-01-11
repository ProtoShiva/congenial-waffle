git config --list //fetch all the config list

git config --global user.name "yourname"

when we commit, we take snapshot and files are now added in our local repo

git log //to show all commit

git diff //compare current file with last commit

git help //to find the various commands

git rm <filename> //remove a file

git rm -r <directory>

git ls-files //see all the files in repo

# Tagging

tag diff points in history . eg tagging in commit history

git tag <tagname>
eg: git tag version1
git tag v1.1

git tag --list //show all the tags

git tag -l <search query> //to find a particular tag
eg: git tag -l "v1\*" //finds all tags containing v1

git tag -a <tagname> -m "any messagge you want"
eg: git tag -a v2.2 -m "this is version 2"

git show <tagname> //fetch all the details of the tagged commit

git tag --delete <tagname>

# unstaged file

git restore --staged <filename>
OR
git reset HEAD <filename>

# unmodifying files

cat <filename> //to see content of files
vi <filename> //we can put content inside files

changes you made since last commit, you don't need it

git restore <filename> //discard the changes you made

# github : remote vcs

to push local repo in github

1. git remote add origin https://github.com/ProtoShiva/congenial-waffle.git

origin is alias or nickname of our repo, so that instead of using the whole url we can use 'origin' as shortcut

git remote
git remote -v

2. git branch -M main

3. git push -u origin main

# SSH

secure shell: it helps in managing remote server and providing the ablility to safely connect and log and work from anywhere.
it makes secure remote connection.
problem with remote connection: vulnerable, hackers can sniff data
data over the network should be encrypted for secure connection
so ssh protocol provide robust encryption using cryptographic algos

in github we can create SSH keys to make a secure connection

for clone and pull in private repo we need authentication

for pushing we need auth in both public and private
auth can be https or ssh

# watch star

watching: notified whenever changes made in your favourite repos
star: bookmark fav repos

# raw blame

go to a repo , open a file, if you want to copy that file just use 'Raw' button

'Blame': to tell you who made what changes in that code file

'history': shows history of commits for that particular file in the project

# issues

they are like todo list for a project.
you can label, assign someone, describe the issue by creating new issue

# fork and pr

fork means to work on a repo, just copy it into your account, do changes in any file and make a Pull request

# clone

if you want to work on a repo locally whereas in fork a copy is created on Github

git clone https://github.com/rajaraodv/react-redux-blog.git

now locally on vscode we can make changes and push code in remote repo.
if author allows us to push we can push and create PRs

# Branches

we don't want to push changes on main or master branch.
Use additional branches to do so. They are like version of your code.
So the changes don't affect our main code.

git branch <branchName> //the data of master branch is copied on this branch

git branch //to display all the branches

git checkout adding-feature // switch to this branch
