
Muthu@THE_RAIN MINGW32 /d/github
$ git init
Initialized empty Git repository in D:/github/.git/

Muthu@THE_RAIN MINGW32 /d/github (master)
$ git remote add orgin "https://github.com/mvravce/git-github.git"

Muthu@THE_RAIN MINGW32 /d/github (master)
$ git pull orgin master
remote: Counting objects: 6, done.
remote: Compressing objects: 100% (2/2), done.
remote: Total 6 (delta 0), reused 0 (delta 0), pack-reused 0
Unpacking objects: 100% (6/6), done.
From https://github.com/mvravce/git-github
 * branch            master     -> FETCH_HEAD
 * [new branch]      master     -> orgin/master

Muthu@THE_RAIN MINGW32 /d/github (master)
$ git status
On branch master
nothing to commit, working tree clean

Muthu@THE_RAIN MINGW32 /d/github (master)
$ git status
On branch master
Untracked files:
  (use "git add <file>..." to include in what will be committed)

        hello.txt

nothing added to commit but untracked files present (use "git add" to track)

Muthu@THE_RAIN MINGW32 /d/github (master)
$ git add hello.txt

Muthu@THE_RAIN MINGW32 /d/github (master)
$ git status
On branch master
Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)

        new file:   hello.txt


Muthu@THE_RAIN MINGW32 /d/github (master)
$ git commit -m "added new file"

*** Please tell me who you are.

Run

  git config --global user.email "you@example.com"
  git config --global user.name "Your Name"

to set your account's default identity.
Omit --global to set the identity only in this repository.

fatal: unable to auto-detect email address (got 'Muthu@THE_RAIN.(none)')

Muthu@THE_RAIN MINGW32 /d/github (master)
$ git commit -m "added new file"

*** Please tell me who you are.

Run

  git config --global user.email "you@example.com"
  git config --global user.name "Your Name"

to set your account's default identity.
Omit --global to set the identity only in this repository.

fatal: unable to auto-detect email address (got 'Muthu@THE_RAIN.(none)')

Muthu@THE_RAIN MINGW32 /d/github (master)
$ git status
On branch master
Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)

        new file:   hello.txt


Muthu@THE_RAIN MINGW32 /d/github (master)
$ git commit -m "added new file"

*** Please tell me who you are.

Run

  git config --global user.email "you@example.com"
  git config --global user.name "Your Name"

to set your account's default identity.
Omit --global to set the identity only in this repository.

fatal: unable to auto-detect email address (got 'Muthu@THE_RAIN.(none)')

Muthu@THE_RAIN MINGW32 /d/github (master)
$ git config --global user.email "mvr_avce@yahoo.co.in"

Muthu@THE_RAIN MINGW32 /d/github (master)
$ git config --global user.name "mvravce"

Muthu@THE_RAIN MINGW32 /d/github (master)
$ git commit -m "added new file"
[master 07ecf95] added new file
 1 file changed, 1 insertion(+)
 create mode 100644 hello.txt

Muthu@THE_RAIN MINGW32 /d/github (master)
$ git status
On branch master
Untracked files:
  (use "git add <file>..." to include in what will be committed)

        hello1.txt
        hello2.txt

nothing added to commit but untracked files present (use "git add" to track)

Muthu@THE_RAIN MINGW32 /d/github (master)
$ git status
On branch master
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)

        modified:   hello.txt

Untracked files:
  (use "git add <file>..." to include in what will be committed)

        hello1.txt
        hello2.txt

no changes added to commit (use "git add" and/or "git commit -a")

Muthu@THE_RAIN MINGW32 /d/github (master)
$ git add -A

Muthu@THE_RAIN MINGW32 /d/github (master)
$ git status
On branch master
Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)

        modified:   hello.txt
        new file:   hello1.txt
        new file:   hello2.txt


Muthu@THE_RAIN MINGW32 /d/github (master)
$ git commit -a -m "commiting all files"
[master 6fb0a3a] commiting all files
 3 files changed, 5 insertions(+), 1 deletion(-)
 create mode 100644 hello1.txt
 create mode 100644 hello2.txt

Muthu@THE_RAIN MINGW32 /d/github (master)
$ git status
On branch master
nothing to commit, working tree clean

Muthu@THE_RAIN MINGW32 /d/github (master)
$ git log
commit 6fb0a3acf21e62ff765172aa0ea7a08ba25a29cd (HEAD -> master)
Author: mvravce <mvr_avce@yahoo.co.in>
Date:   Sat Jun 17 12:33:50 2017 +0530

    commiting all files

commit 07ecf95c7fd0d0f965a37aa4afac61cbe1313a58
Author: mvravce <mvr_avce@yahoo.co.in>
Date:   Sat Jun 17 12:31:11 2017 +0530

    added new file

commit f256eabfd19ecdace593f609fc469b6afae71e99 (orgin/master)
Author: mvravce <mvr_avce@yahoo.co.in>
Date:   Sat Jun 17 12:07:54 2017 +0530

    Update README.md

commit df129b6485f95225c52c598550585fbbfa222da9
Author: mvravce <mvr_avce@yahoo.co.in>
Date:   Sat Jun 17 12:06:54 2017 +0530

    Initial commit
:

Muthu@THE_RAIN MINGW32 /d/github (master)
git branch firstbranch

Muthu@THE_RAIN MINGW32 /d/github (master)
$ git checkout firstbranch
Switched to branch 'firstbranch'

Muthu@THE_RAIN MINGW32 /d/github (firstbranch)
$ git add -A

Muthu@THE_RAIN MINGW32 /d/github (firstbranch)
$ git status
On branch firstbranch
Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)

        new file:   hellobranch.txt


Muthu@THE_RAIN MINGW32 /d/github (firstbranch)
$ git commit  -m "newbranch file"
[firstbranch 01fb95f] newbranch file
 1 file changed, 1 insertion(+)
 create mode 100644 hellobranch.txt

Muthu@THE_RAIN MINGW32 /d/github (firstbranch)
$ git checkout master
Switched to branch 'master'

Muthu@THE_RAIN MINGW32 /d/github (master)
$ ls
hello.txt  hello1.txt  hello2.txt  README.md

Muthu@THE_RAIN MINGW32 /d/github (master)
$ git checkout firstbranch
Switched to branch 'firstbranch'

Muthu@THE_RAIN MINGW32 /d/github (firstbranch)
$ ls
hello.txt  hello1.txt  hello2.txt  hellobranch.txt  README.md

Muthu@THE_RAIN MINGW32 /d/github (firstbranch)
$ git checkout master
Switched to branch 'master'

Muthu@THE_RAIN MINGW32 /d/github (master)
$ git merge firstbranch
Updating 6fb0a3a..01fb95f
Fast-forward
 hellobranch.txt | 1 +
 1 file changed, 1 insertion(+)
 create mode 100644 hellobranch.txt

Muthu@THE_RAIN MINGW32 /d/github (master)
$ ls
hello.txt  hello1.txt  hello2.txt  hellobranch.txt  README.md

Muthu@THE_RAIN MINGW32 /d/github (master)
$ git checkout firstbranch
Switched to branch 'firstbranch'

Muthu@THE_RAIN MINGW32 /d/github (firstbranch)
$ git commit -a -m "change hellobranch"
[firstbranch e383854] change hellobranch
 1 file changed, 1 insertion(+), 1 deletion(-)

Muthu@THE_RAIN MINGW32 /d/github (firstbranch)
$ git checkout master
Switched to branch 'master'

Muthu@THE_RAIN MINGW32 /d/github (master)
$ git merge firstbranch
Updating 01fb95f..e383854
Fast-forward
 hellobranch.txt | 2 +-
 1 file changed, 1 insertion(+), 1 deletion(-)

Muthu@THE_RAIN MINGW32 /d/github (master)
$ cat hellobranch.txt
first branch, modified in firts branch
Muthu@THE_RAIN MINGW32 /d/github (master)
$ git checkout firstbranch
Switched to branch 'firstbranch'

Muthu@THE_RAIN MINGW32 /d/github (firstbranch)
$ cat hellobranch.txt
first branch, modified in firts branch
Muthu@THE_RAIN MINGW32 /d/github (firstbranch)
$ git add -A

Muthu@THE_RAIN MINGW32 /d/github (firstbranch)
$ git commit -a -m "addedc two file more"
[firstbranch 5f285d0] addedc two file more
 2 files changed, 2 insertions(+)
 create mode 100644 branch2.txt
 create mode 100644 branch3.txt

Muthu@THE_RAIN MINGW32 /d/github (firstbranch)
$ ls
branch2.txt  branch3.txt  hello.txt  hello1.txt  hello2.txt  hellobranch.txt  README.md

Muthu@THE_RAIN MINGW32 /d/github (firstbranch)
$ git checkout master
Switched to branch 'master'

Muthu@THE_RAIN MINGW32 /d/github (master)
$ ls
hello.txt  hello1.txt  hello2.txt  hellobranch.txt  README.md

Muthu@THE_RAIN MINGW32 /d/github (master)
$ git checkout firstbranch
Switched to branch 'firstbranch'

Muthu@THE_RAIN MINGW32 /d/github (firstbranch)
$ git rebase master
Current branch firstbranch is up to date.

Muthu@THE_RAIN MINGW32 /d/github (firstbranch)
$ git checkout master
Switched to branch 'master'

Muthu@THE_RAIN MINGW32 /d/github (master)
$ git rebase firstbranch
First, rewinding head to replay your work on top of it...
Fast-forwarded master to firstbranch.

Muthu@THE_RAIN MINGW32 /d/github (master)
$ ls
branch2.txt  branch3.txt  hello.txt  hello1.txt  hello2.txt  hellobranch.txt  README.md

Muthu@THE_RAIN MINGW32 /d/github (master)
$ ssh-keygen
Generating public/private rsa key pair.
Enter file in which to save the key (/c/Users/Muthu/.ssh/id_rsa):
Created directory '/c/Users/Muthu/.ssh'.
Enter passphrase (empty for no passphrase):
Enter same passphrase again:
Your identification has been saved in /c/Users/Muthu/.ssh/id_rsa.
Your public key has been saved in /c/Users/Muthu/.ssh/id_rsa.pub.
The key fingerprint is:
SHA256:dioJEftPOk3fXlTnlyl1efHrAk0LP8GAj3SUXhMxHK8 Muthu@THE_RAIN
The key's randomart image is:
+---[RSA 2048]----+
|    .     ooo=+. |
|     o   o oo+o +|
|    o   . =..+.+*|
|     o   . o= =oB|
|    . . S .. E.+o|
|     . O + ...+ .|
|      = + . .... |
|       o   . ..  |
|            .    |
+----[SHA256]-----+

Muthu@THE_RAIN MINGW32 /d/github (master)
$ cat c/Users/Muthu/.ssh/id_rsa.pub
cat: c/Users/Muthu/.ssh/id_rsa.pub: No such file or directory

Muthu@THE_RAIN MINGW32 /d/github (master)
$ cat c/Users/Muthu/.ssh/id_rsa.pub.
cat: c/Users/Muthu/.ssh/id_rsa.pub.: No such file or directory

Muthu@THE_RAIN MINGW32 /d/github (master)
$ cat /c/Users/Muthu/.ssh/id_rsa.pub.
cat: /c/Users/Muthu/.ssh/id_rsa.pub.: No such file or directory

Muthu@THE_RAIN MINGW32 /d/github (master)
$ cat C:\Users\Muthu\.ssh\id_rsa.pub
cat: 'C:UsersMuthu.sshid_rsa.pub': No such file or directory

Muthu@THE_RAIN MINGW32 /d/github (master)
$ ssh -T git@git-hub.com
ssh: connect to host git-hub.com port 22: Connection timed out

Muthu@THE_RAIN MINGW32 /d/github (master)
$ ssh -T git@git-hub.com
ssh: connect to host git-hub.com port 22: Connection timed out

Muthu@THE_RAIN MINGW32 /d/github (master)
$ ssh -T git@github.com
The authenticity of host 'github.com (192.30.253.112)' can't be established.
RSA key fingerprint is SHA256:nThbg6kXUpJWGl7E1IGOCspRomTxdCARLviKw6E5SY8.
Are you sure you want to continue connecting (yes/no)?
Host key verification failed.

Muthu@THE_RAIN MINGW32 /d/github (master)
$ ssh -T git@github.com
The authenticity of host 'github.com (192.30.253.112)' can't be established.
RSA key fingerprint is SHA256:nThbg6kXUpJWGl7E1IGOCspRomTxdCARLviKw6E5SY8.
Are you sure you want to continue connecting (yes/no)? y
Please type 'yes' or 'no': yes
Warning: Permanently added 'github.com,192.30.253.112' (RSA) to the list of known hosts.
Hi mvravce! You've successfully authenticated, but GitHub does not provide shell access.

Muthu@THE_RAIN MINGW32 /d/github (master)
$ git checkout firstbranch
Switched to branch 'firstbranch'

Muthu@THE_RAIN MINGW32 /d/github (firstbranch)
$ git push orgin firstbranch
Counting objects: 18, done.
Delta compression using up to 4 threads.
Compressing objects: 100% (10/10), done.
Writing objects: 100% (18/18), 1.35 KiB | 0 bytes/s, done.
Total 18 (delta 3), reused 0 (delta 0)
remote: Resolving deltas: 100% (3/3), done.
To https://github.com/mvravce/git-github.git
 * [new branch]      firstbranch -> firstbranch

Muthu@THE_RAIN MINGW32 /d/github (firstbranch)
$ git checkout master
Switched to branch 'master'

Muthu@THE_RAIN MINGW32 /d/github (master)
$ git push orgin master
Total 0 (delta 0), reused 0 (delta 0)
To https://github.com/mvravce/git-github.git
   f256eab..5f285d0  master -> master

Muthu@THE_RAIN MINGW32 /d/github (master)
$ git add revert.txt
bash: $'\302\201\302\201git': command not found

Muthu@THE_RAIN MINGW32 /d/github (master)
$ git add revert.txt
bash: $'\302\201\302\201git': command not found

Muthu@THE_RAIN MINGW32 /d/github (master)
$ git status
On branch master
Untracked files:
  (use "git add <file>..." to include in what will be committed)

        revert.txt

nothing added to commit but untracked files present (use "git add" to track)

Muthu@THE_RAIN MINGW32 /d/github (master)
$ git add revert.txt
bash: $'\302\201\302\201git': command not found

Muthu@THE_RAIN MINGW32 /d/github (master)
$ git add "revert.txt"
bash: $'\302\201\302\201git': command not found

Muthu@THE_RAIN MINGW32 /d/github (master)
$ git add -A
bash: $'\302\201\302\201git': command not found

Muthu@THE_RAIN MINGW32 /d/github (master)
$ git status
On branch master
Untracked files:
  (use "git add <file>..." to include in what will be committed)

        revert.txt

nothing added to commit but untracked files present (use "git add" to track)

Muthu@THE_RAIN MINGW32 /d/github (master)
$ git add revert.txt
bash: $'\302\201\302\201git': command not found

Muthu@THE_RAIN MINGW32 /d/github (master)
$ git checkout master
Already on 'master'

Muthu@THE_RAIN MINGW32 /d/github (master)
$ git add revert.txtr
bash: $'\302\201\302\201git': command not found

Muthu@THE_RAIN MINGW32 /d/github (master)
$ git checkout firstbranch
Switched to branch 'firstbranch'

Muthu@THE_RAIN MINGW32 /d/github (firstbranch)
$ git add revert.txtch
bash: $'\302\201\302\201git': command not found

Muthu@THE_RAIN MINGW32 /d/github (firstbranch)
$ git add revert.txt
bash: $'\302\201\302\201git': command not found

Muthu@THE_RAIN MINGW32 /d/github (firstbranch)
$ git checkout firstbranch

Muthu@THE_RAIN MINGW32 /d/github (firstbranch)
$ git checkout master
Switched to branch 'master'
M       README.md

Muthu@THE_RAIN MINGW32 /d/github (master)
$ git status
On branch master
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)

        modified:   README.md

Untracked files:
  (use "git add <file>..." to include in what will be committed)

        revert.txt

no changes added to commit (use "git add" and/or "git commit -a")

Muthu@THE_RAIN MINGW32 /d/github (master)
$ git add revert.txt

Muthu@THE_RAIN MINGW32 /d/github (master)
$ git commit -m "revert.txt"
[master 4bb3b1d] revert.txt
 1 file changed, 1 insertion(+)
 create mode 100644 revert.txt

Muthu@THE_RAIN MINGW32 /d/github (master)
$ git commit -a -m "reverttt"
[master 081dc3a] reverttt
 2 files changed, 478 insertions(+), 3 deletions(-)
 rewrite README.md (100%)

Muthu@THE_RAIN MINGW32 /d/github (master)
$ git log
commit 081dc3a0e5c87d1146733a4b4bf64869f38d2fa3 (HEAD -> master)
Author: mvravce <mvr_avce@yahoo.co.in>
Date:   Sat Jun 17 13:29:54 2017 +0530

    reverttt

commit 4bb3b1dca9fe65f9b926622d35806d05b585212c
Author: mvravce <mvr_avce@yahoo.co.in>
Date:   Sat Jun 17 13:28:52 2017 +0530

    revert.txt

commit 5f285d08a24725b797dc052ee72169197ca3553d (orgin/master, orgin/firstbranch                                                                                                                , firstbranch)
Author: mvravce <mvr_avce@yahoo.co.in>
Date:   Sat Jun 17 12:53:14 2017 +0530

    addedc two file more

commit e38385457e5af07fa20df39f3045ae943e504c78
Author: mvravce <mvr_avce@yahoo.co.in>
Date:   Sat Jun 17 12:46:02 2017 +0530

:

Muthu@THE_RAIN MINGW32 /d/github (master)
 checkout Date:   Sat Jun 17 12:53:14 2017 +0530


bash: gi: command not found

Muthu@THE_RAIN MINGW32 /d/github (master)
$ Date:   Sat Jun 17 12:53:14 2017 +0530
bash: Date:: command not found

Muthu@THE_RAIN MINGW32 /d/github (master)
$

Muthu@THE_RAIN MINGW32 /d/github (master)
$ git checkout


Muthu@THE_RAIN MINGW32 /d/github (master)
$ Date:   Sat Jun 17 12:53:14 2017 +0530
bash: Date:: command not found

Muthu@THE_RAIN MINGW32 /d/github (master)
$

Muthu@THE_RAIN MINGW32 /d/github (master)
$ git log
commit 081dc3a0e5c87d1146733a4b4bf64869f38d2fa3 (HEAD -> master)
Author: mvravce <mvr_avce@yahoo.co.in>
Date:   Sat Jun 17 13:29:54 2017 +0530

    reverttt

commit 4bb3b1dca9fe65f9b926622d35806d05b585212c
Author: mvravce <mvr_avce@yahoo.co.in>
Date:   Sat Jun 17 13:28:52 2017 +0530

    revert.txt

commit 5f285d08a24725b797dc052ee72169197ca3553d (orgin/master, orgin/firstbranch                                                                                                                , firstbranch)
Author: mvravce <mvr_avce@yahoo.co.in>
Date:   Sat Jun 17 12:53:14 2017 +0530

    addedc two file more

commit e38385457e5af07fa20df39f3045ae943e504c78
Author: mvravce <mvr_avce@yahoo.co.in>
Date:   Sat Jun 17 12:46:02 2017 +0530

:

Muthu@THE_RAIN MINGW32 /d/github (master)
git checkout 4bb3b1dc "revert.txt"
bash: t: command not found

Muthu@THE_RAIN MINGW32 /d/github (master)
$ t checkout 4bb3b1dc revert.txt
bash: t: command not found

Muthu@THE_RAIN MINGW32 /d/github (master)
$ git checkout 4bb3b1dc revert.txt

Muthu@THE_RAIN MINGW32 /d/github (master)
$ cat revert.txt
revert file
Muthu@THE_RAIN MINGW32 /d/github (master)
$

