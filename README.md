# GIT Exercises

## Bundle 1

### Exercise 1

```bash

user@LAPTOP-GQ4K54L5 MINGW64 ~
$ mkdir myproject

user@LAPTOP-GQ4K54L5 MINGW64 ~
$ cd myproject

user@LAPTOP-GQ4K54L5 MINGW64 ~/myproject
$ git init
Initialized empty Git repository in C:/Users/user/myproject/.git/

user@LAPTOP-GQ4K54L5 MINGW64 ~/myproject (master)
$ code .

user@LAPTOP-GQ4K54L5 MINGW64 ~/myproject (master)
$ git branch -m master main

user@LAPTOP-GQ4K54L5 MINGW64 ~/myproject (main)
$ git add --all

user@LAPTOP-GQ4K54L5 MINGW64 ~/myproject (main)
$ git commit -m 'First Edition No Change Yet'
[main (root-commit) 57761d2] First Edition No Change Yet
 1 file changed, 12 insertions(+)
 create mode 100644 index.html

user@LAPTOP-GQ4K54L5 MINGW64 ~/myproject (main)
$ ls ~/.ssh
ls: cannot access '/c/Users/user/.ssh': No such file or directory

user@LAPTOP-GQ4K54L5 MINGW64 ~/myproject (main)
$ ssh-keygen -t rsa -b 4096 -C "igiranezatheogene4@gmail.com"
Generating public/private rsa key pair.
Enter file in which to save the key (/c/Users/user/.ssh/id_rsa):
Created directory '/c/Users/user/.ssh'.
Enter passphrase for "/c/Users/user/.ssh/id_rsa" (empty for no passphrase):
Enter same passphrase again:
Your identification has been saved in /c/Users/user/.ssh/id_rsa
Your public key has been saved in /c/Users/user/.ssh/id_rsa.pub
The key fingerprint is:
SHA256:wUnSYmtZkdHfLXWmAnm9pr14nkpcB+c+tr5BsAt/Vog igiranezatheogene4@gmail.com
The key's randomart image is:
+---[RSA 4096]----+
|      ..+= . .   |
|      o++.+ . . +|
|     . =+  + o.*o|
|      +  .  o.O=.|
|     .  S  .E*oo+|
|           .+.+o.|
|            o+ B.|
|           .. *.+|
|            .+++.|
+----[SHA256]-----+

user@LAPTOP-GQ4K54L5 MINGW64 ~/myproject (main)
$ eval "$(ssh-agent -s)"
Agent pid 755

user@LAPTOP-GQ4K54L5 MINGW64 ~/myproject (main)
$ ssh-add ~/.ssh/id_rsa
Identity added: /c/Users/user/.ssh/id_rsa (igiranezatheogene4@gmail.com)

user@LAPTOP-GQ4K54L5 MINGW64 ~/myproject (main)
$ clip < ~/.ssh/id_rsa.pub

user@LAPTOP-GQ4K54L5 MINGW64 ~/myproject (main)
$ ssh -T git@github.com
The authenticity of host 'github.com (20.87.245.0)' can't be established.
ED25519 key fingerprint is SHA256:+DiY3wvvV6TuJJhbpZisF/zLDA0zPMSvHdkr4UvCOqU.
This key is not known by any other names.
Are you sure you want to continue connecting (yes/no/[fingerprint])? yes
Warning: Permanently added 'github.com' (ED25519) to the list of known hosts.
Hi Theogene120! You've successfully authenticated, but GitHub does not provide shell access.

user@LAPTOP-GQ4K54L5 MINGW64 ~/myproject (main)
$ git remote add origin git@github.com:Theogene120/Gym-Git-Exercise-Solutions

user@LAPTOP-GQ4K54L5 MINGW64 ~/myproject (main)
$ git pull origin main --rebase
From github.com:Theogene120/Gym-Git-Exercise-Solutions
 * branch            main       -> FETCH_HEAD
Successfully rebased and updated refs/heads/main.

user@LAPTOP-GQ4K54L5 MINGW64 ~/myproject (main)
$ git push -u origin main
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 16 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 493 bytes | 493.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To github.com:Theogene120/Gym-Git-Exercise-Solutions
   8e1f90f..4df7347  main -> main
branch 'main' set up to track 'origin/main'.

user@LAPTOP-GQ4K54L5 MINGW64 ~/myproject (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        README-local-backup.md

nothing added to commit but untracked files present (use "git add" to track)

user@LAPTOP-GQ4K54L5 MINGW64 ~/myproject (main)
$ git branch dev

user@LAPTOP-GQ4K54L5 MINGW64 ~/myproject (main)
$ git checkout dev
Switched to branch 'dev'

user@LAPTOP-GQ4K54L5 MINGW64 ~/myproject (dev)
$ git branch test

user@LAPTOP-GQ4K54L5 MINGW64 ~/myproject (dev)
$ git branch -d test
Deleted branch test (was 4df7347).

user@LAPTOP-GQ4K54L5 MINGW64 ~/myproject (dev)
$ git branch
* dev
  main

user@LAPTOP-GQ4K54L5 MINGW64 ~/myproject (dev)
$
```