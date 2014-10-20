#1. First Use Setup
yin@WorkLap:~/Gits/learn_git$ git config --global user.name "Yin Zixin"

yin@WorkLap:~/Gits/learn_git$ git config --global user.email "yinzixin1985@hotmail.com"

yin@WorkLap:~/Gits/learn_git$ git config --global core.editor vim

#2. Clone a remoting repository

```
yin@WorkLap:~/Gits$ git clone https://github.com/yinzixin/learn_git.gitCloning into 'learn_git'...
remote: Counting objects: 3, done.
remote: Total 3 (delta 0), reused 0 (delta 0)
Unpacking objects: 100% (3/3), done.
Checking connectivity... done.
```
This will create a folder.

```
yin@WorkLap:~/Gits$ ls
learn_git
```

#3. Show Status of a repository
yin@WorkLap:~/Gits/learn_git$ git status
On branch master
Your branch is up-to-date with 'origin/master'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)

	fast_tuto.txt

nothing added to commit but untracked files present (use "git add" to track)

#4. Stage Changed file 
yin@WorkLap:~/Gits/learn_git$ git add fast_tuto.txt
yin@WorkLap:~/Gits/learn_git$ git status
On branch master
Your branch is up-to-date with 'origin/master'.

Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)

	new file:   fast_tuto.txt

#5. Commit staged file
	git commit

#6. Push commited changes to remote server
yin@WorkLap:~/Gits/learn_git$ git push origin master
Username for 'https://github.com': yinzixin1985@hotmail.com
Password for 'https://yinzixin1985@hotmail.com@github.com': 
Counting objects: 4, done.
Delta compression using up to 4 threads.
Compressing objects: 100% (2/2), done.
Writing objects: 100% (4/4), 297 bytes | 0 bytes/s, done.
Total 4 (delta 0), reused 0 (delta 0)
To https://github.com/yinzixin/Notes.git
 * [new branch]      master -> master

If you use https to push changes, it will ask you to input your user name and password.
Use config to set password cache and timeout (second) of the cache.
 git config --global credential.helper 'cache --timeout=864000'


#7. rename
 git mv fast_tuto.txt fast_tuto.md

TODO:
4. learn more about gist
