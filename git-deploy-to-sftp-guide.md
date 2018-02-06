# Guide to use git to deploy via sftp

#### this method can be used to push your project to a service like GoDaddy, HostGator, or BlueHost that is running git.


- create a remote repository on your server

  - ssh into the server

  - cd into the directory

```
mkdir .git
cd .git
git init --bare
cd hooks
touch post-receive
chmod +x post-receive
```

  - paste this into the post-receive file you just created, replace path with your project directory

```
#!/bin/sh
GIT_WORK_TREE=/home/user/public_html/your-dir git checkout -f
```

---------------------------

- now we add the remote repository to our local dev project

```
git remote add bluehost user@your_domain.com:/home/user/public_html/your_dir/.git
git add -all
git status
git commit -m "added text file"
//if also hosted on github etc
git push -u origin master

//push to new repo
git push -u bluehost master

```

https://stackoverflow.com/questions/17876843/how-to-push-to-both-github-and-live-server-from-local-repository
