```bash
brew install gh
```
install gh cli

```bash
gh auth login
```
Login my get hub user to gh
### Terminal Output
```
 Where do you use GitHub? 
 GitHub.com?
 
 What is your preferred protocol for Git operations on this host? HTTPS?

 Authenticate Git with your GitHub credentials? Yes?
How would you like to authenticate GitHub CLI? Login with a web browser
First copy your one-time code: 7432-F567
Press Enter to open https://github.com/login/device in your browser... 
Gtk-Message: 12:09:34.745: Not loading module "atk-bridge": The functionality is provided by GTK natively. Please try to not load it.
✓ Authentication complete.
- gh config set -h github.com git_protocol https
✓ Configured git protocol
✓ Logged in as DRLopez26
```

```
rey@fox:~/repo$ gh repo clone https://github.com/aviusly/notes
Cloning into 'notes'...
remote: Enumerating objects: 6, done.
remote: Counting objects: 100% (6/6), done.
remote: Compressing objects: 100% (5/5), done.
remote: Total 6 (delta 0), reused 6 (delta 0), pack-reused 0 (from 0)
Receiving objects: 100% (6/6), done.
rey@fox:~/repo$ cd notes
rey@fox:~/repo/notes$ ls
cmdpython.sh  editpath.md  newuser.md  sed.md
rey@fox:~/repo/notes$ touch gh.md
rey@fox:~/repo/notes$ ls
cmdpython.sh  editpath.md  gh.md  newuser.md  sed.md
rey@fox:~/repo/notes$ code gh.md 
rey@fox:~/repo/notes$ code editpath.md 
rey@fox:~/repo/notes$ cd
rey@fox:~$ ls
Desktop  Documents  Downloads  helloworld.py  Music  Pictures  Public  repo  snap  Templates  Videos
rey@fox:~$ cd repo
rey@fox:~/repo$ ls
notes
rey@fox:~/repo$ cd notes
rey@fox:~/repo/notes$ cd


rey@fox:~/repo$ cd notes
rey@fox:~/repo/notes$ git config --global user.name "Dr Lopez"
rey@fox:~/repo/notes$ git config --global user.email 
rey@fox:~/repo/notes$ git checkout -b drey
Switched to a new branch 'drey'
```

rey@fox:~/repo/notes$ git branch
* drey
  master
rey@fox:~/repo/notes$ gif add.
Command 'gif' not found, did you mean:
  command 'kif' from snap kif (0.2.0)
  command 'ngif' from snap ngif (2.3.51-beta)
  command 'gie' from deb proj-bin (8.2.1-1)
  command 'gid' from deb id-utils (4.6.28-20200521ss15dab)
  command 'uif' from deb uif (1.1.9-5)
  command 'gsf' from deb libgsf-bin (1.14.47-1ubuntu0.1)
  command 'gtf' from deb xserver-xorg-core (2:21.1.4-2ubuntu1.7~22.04.16)
  command 'gio' from deb libglib2.0-bin (2.72.4-0ubuntu2.9)
  command 'git' from deb git (1:2.34.1-1ubuntu1.17)
  command 'tgif' from deb tgif (1:4.2.5-1.3build2)
  command 'gip' from deb gip (1.7.0-1-5)
See 'snap info <snapname>' for additional versions.
rey@fox:~/repo/notes$ gif add.
Command 'gif' not found, did you mean:
  command 'kif' from snap kif (0.2.0)
  command 'ngif' from snap ngif (2.3.51-beta)
  command 'gid' from deb id-utils (4.6.28-20200521ss15dab)
  command 'git' from deb git (1:2.34.1-1ubuntu1.17)
  command 'gie' from deb proj-bin (8.2.1-1)
  command 'gip' from deb gip (1.7.0-1-5)
  command 'gsf' from deb libgsf-bin (1.14.47-1ubuntu0.1)
  command 'uif' from deb uif (1.1.9-5)
  command 'gtf' from deb xserver-xorg-core (2:21.1.4-2ubuntu1.7~22.04.16)
  command 'gio' from deb libglib2.0-bin (2.72.4-0ubuntu2.9)
  command 'tgif' from deb tgif (1:4.2.5-1.3build2)
See 'snap info <snapname>' for additional versions.
rey@fox:~/repo/notes$ git commit -m "one small step"
On branch drey
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        gh.md

nothing added to commit but untracked files present (use "git add" to track)
rey@fox:~/repo/notes$ git push
fatal: The current branch drey has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin drey

rey@fox:~/repo/notes$ git push --set-upstream origin drey
remote: Permission to aviusly/notes.git denied to DRLopez26.
fatal: unable to access 'https://github.com/aviusly/notes.git/': The requested URL returned error: 403
rey@fox:~/repo/notes$ 
