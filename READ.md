## Git Tutorial


TO check Git version and installation of the git 

```
git --version

```

# Config your Github username and Email

Config username

```
git config --global user.name "your github username"
```

Config Email ID

```
git config --global user.email "your email id"

```

To check your Config detail

```
git config --global user.email
git config --global user.name
```

To make changes in your config detail 

```
git config --global --edit
```

## To create new folder 

```
mkdir yourfilename
```
To change directory 
```
cd yourfilename/
```

 To initialize this folder into github repo

 ```
 git init
 ``` 

To check the list of hidden and created file in your repo

```
ls
ls -a  #show hidden file 
```

To track the changes in your github repo 
```
git status
```
## Staging Area
To track your file for commiting

```
git add filename      #only given file will be track
git add .             #to track all file 
```

## Commit

To commit the tracked file in repo
```
git commit -m "must have any message"
```
To check number of commit
```
git log
```

To check your commit at any particular number of commit 
for this you need your hashcode (To get hashcode run git log command)
```
git checkout <commit hash code/branchname>
```
To go back to your last commit 
```
git checkout master
```
To check your branch 

```
git branch
```
To  create branch 
```
git branch branchname
```
To switch to new branch 
```
git checkout branchname
```
To create and checkout branch at a time
```
git checkout -b abdul/multiple
```
To merge different branch
first checkout to dev then merge
```
git checkout dev
git merge abdul/multiple
```

## .gitignore

To drop any unecessory ignore

first create .gitignore file
```
touch .gitignore
```
### To ignore particular file just write the file name with extension into .gitignore file
### To ignore particular folder foldername/


# Push Repo

```
git remote add origin <github repo link>
```
```
git remote -v
```
To push master branch
```
git branch -M master
```
```
git push -u origin master
```
If you want to push other branches
```
git checkout branch_name
```
```
git push -u origin master
```
or 
```
git push -u origin dev
```


