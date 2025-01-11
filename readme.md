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
