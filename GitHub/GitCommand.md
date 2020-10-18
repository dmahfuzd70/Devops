MAHFUZUR RAHMAN@DESKTOP-4Q0OEE3 MINGW64 ~/Desktop/Devops/GitHub/Project-1

    $ git init

    Initialized empty Git repository in C:/Users/MAHFUZUR RAHMAN/Desktop/Devops/GitHub/Project-1/.git/

MAHFUZUR RAHMAN@DESKTOP-4Q0OEE3 MINGW64 ~/Desktop/Devops/GitHub/Project-1 (master)

    $ git config --global user.name "Mahfuzur Rahman"

MAHFUZUR RAHMAN@DESKTOP-4Q0OEE3 MINGW64 ~/Desktop/Devops/GitHub/Project-1 (master)

    $ git config --global user.email "dmahfuzd@gmail.com"

MAHFUZUR RAHMAN@DESKTOP-4Q0OEE3 MINGW64 ~/Desktop/Devops/GitHub/Project-1 (master)

    $ git config --list

    diff.astextplain.textconv=astextplain
    filter.lfs.clean=git-lfs clean -- %f
    filter.lfs.smudge=git-lfs smudge -- %f
    filter.lfs.process=git-lfs filter-process
    filter.lfs.required=true
    http.sslbackend=openssl
    http.sslcainfo=C:/Program Files/Git/mingw64/ssl/certs/ca-bundle.crt
    core.autocrlf=true
    core.fscache=true
    core.symlinks=false
    pull.rebase=false
    credential.helper=manager
    user.name=Mahfuzur Rahman
    user.email=dmahfuzd@gmail.com
    core.repositoryformatversion=0
    core.filemode=false
    core.bare=false
    core.logallrefupdates=true
    core.symlinks=false
    core.ignorecase=truegit

MAHFUZUR RAHMAN@DESKTOP-4Q0OEE3 MINGW64 ~/Desktop/Devops/GitHub/Project-1 (master)
$


MAHFUZUR RAHMAN@DESKTOP-4Q0OEE3 MINGW64 ~/Desktop/Devops/GitHub/Project-1 (master)
    
    $ git status
    
    On branch master

    No commits yet

    Untracked files:
    (use "git add <file>..." to include in what will be committed)
        cold.txt
        hot.txt

    nothing added to commit but untracked files present (use "git add" to track)

MAHFUZUR RAHMAN@DESKTOP-4Q0OEE3 MINGW64 ~/Desktop/Devops/GitHub/Project-1 (master)
$


MAHFUZUR RAHMAN@DESKTOP-4Q0OEE3 MINGW64 ~/Desktop/Devops/GitHub/Project-1 (master)
 
       $ git add cold.txt

MAHFUZUR RAHMAN@DESKTOP-4Q0OEE3 MINGW64 ~/Desktop/Devops/GitHub/Project-1 (master)

    $ git status
    On branch master

    No commits yet

    Changes to be committed:
      (use "git rm --cached <file>..." to unstage)
            new file:   cold.txt

    Untracked files:
      (use "git add <file>..." to include in what will be committed)
            hot.txt


MAHFUZUR RAHMAN@DESKTOP-4Q0OEE3 MINGW64 ~/Desktop/Devops/GitHub/Project-1 (master)


MAHFUZUR RAHMAN@DESKTOP-4Q0OEE3 MINGW64 ~/Desktop/Devops/GitHub/Project-1 (master)
    
    $ git add --all

MAHFUZUR RAHMAN@DESKTOP-4Q0OEE3 MINGW64 ~/Desktop/Devops/GitHub/Project-1 (master)

    $ git add .

MAHFUZUR RAHMAN@DESKTOP-4Q0OEE3 MINGW64 ~/Desktop/Devops/GitHub/Project-1 (master)
$

  
    $ git commit


    [master (root-commit) 5b41351] Two text file added
     2 files changed, 0 insertions(+), 0 deletions(-)
     create mode 100644 cold.txt
     create mode 100644 hot.txt



MAHFUZUR RAHMAN@DESKTOP-4Q0OEE3 MINGW64 ~/Desktop/Devops/GitHub/Project-1 (master)

    $ git status
    On branch master
    Changes to be committed:
      (use "git restore --staged <file>..." to unstage)
            new file:   chocolate.txt


MAHFUZUR RAHMAN@DESKTOP-4Q0OEE3 MINGW64 ~/Desktop/Devops/GitHub/Project-1 (master)

    $ git commit -m "Chocolate added"
    [master d361a8b] Chocolate added
     1 file changed, 0 insertions(+), 0 deletions(-)
     create mode 100644 chocolate.txt

MAHFUZUR RAHMAN@DESKTOP-4Q0OEE3 MINGW64 ~/Desktop/Devops/GitHub/Project-1 (master)
$

MAHFUZUR RAHMAN@DESKTOP-4Q0OEE3 MINGW64 ~/Desktop/Devops/GitHub/Project-1 (master)

    $ git log
    commit d361a8b4458ef80ceb0f32eb7aa2d33cc558f4b2 (HEAD -> master)
    Author: Mahfuzur Rahman <dmahfuzd@gmail.com>
    Date:   Sat Sep 5 19:20:00 2020 +0600

    Chocolate added

    commit 5b41351f09ae34ef64018d439635745a96ef05fb
    Author: Mahfuzur Rahman <dmahfuzd@gmail.com>
    Date:   Sat Sep 5 19:15:31 2020 +0600

    Two text file added

MAHFUZUR RAHMAN@DESKTOP-4Q0OEE3 MINGW64 ~/Desktop/Devops/GitHub/Project-1 (master)

    $ git log --oneline
    d361a8b (HEAD -> master) Chocolate added
    5b41351 Two text file added

MAHFUZUR RAHMAN@DESKTOP-4Q0OEE3 MINGW64 ~/Desktop/Devops/GitHub/Project-1 (master)
$


    $ git checkout d361a8b
    Note: switching to 'd361a8b'.

    You are in 'detached HEAD' state. You can look around, make experimental
    changes and commit them, and you can discard any commits you make in this
    state without impacting any branches by switching back to a branch.

    If you want to create a new branch to retain commits you create, you may
    do so (now or later) by using -c with the switch command. Example:

      git switch -c <new-branch-name>

    Or undo this operation with:

      git switch -

    Turn off this advice by setting config variable advice.detachedHead to false

    HEAD is now at d361a8b Chocolate added


MAHFUZUR RAHMAN@DESKTOP-4Q0OEE3 MINGW64 ~/Desktop/Devops/GitHub/Project-1 ((d361a8b...))

    $ git status
    HEAD detached at d361a8b
    nothing to commit, working tree clean

MAHFUZUR RAHMAN@DESKTOP-4Q0OEE3 MINGW64 ~/Desktop/Devops/GitHub/Project-1 ((d361a8b...))

    $ git checkout master
    Previous HEAD position was d361a8b Chocolate added
    Switched to branch 'master'

MAHFUZUR RAHMAN@DESKTOP-4Q0OEE3 MINGW64 ~/Desktop/Devops/GitHub/Project-1 (master)
$


MAHFUZUR RAHMAN@DESKTOP-4Q0OEE3 MINGW64 ~/Desktop/Devops/GitHub/Project-1 (master)

    $ git status
    On branch master
    Changes not staged for commit:
      (use "git add <file>..." to update what will be committed)
      (use "git restore <file>..." to discard changes in working directory)
            modified:   chocolate.txt

    no changes added to commit (use "git add" and/or "git commit -a")

MAHFUZUR RAHMAN@DESKTOP-4Q0OEE3 MINGW64 ~/Desktop/Devops/GitHub/Project-1 (master)

    $ git diff
    diff --git a/chocolate.txt b/chocolate.txt
    index e69de29..82f6c81 100644
    --- a/chocolate.txt
    +++ b/chocolate.txt
    @@ -0,0 +1 @@
    +Some Chocolate added.
    \ No newline at end of file

MAHFUZUR RAHMAN@DESKTOP-4Q0OEE3 MINGW64 ~/Desktop/Devops/GitHub/Project-1 (master)


MAHFUZUR RAHMAN@DESKTOP-4Q0OEE3 MINGW64 ~/Desktop/Devops/GitHub/Project-1 (master)

    $ git log --oneline
    7367e81 (HEAD -> master) ice cube added
    d361a8b Chocolate added
    5b41351 Two text file added

MAHFUZUR RAHMAN@DESKTOP-4Q0OEE3 MINGW64 ~/Desktop/Devops/GitHub/Project-1 (master)

    $ git show d361a8b
    commit d361a8b4458ef80ceb0f32eb7aa2d33cc558f4b2
    Author: Mahfuzur Rahman <dmahfuzd@gmail.com>
    Date:   Sat Sep 5 19:20:00 2020 +0600

        Chocolate added

    diff --git a/chocolate.txt b/chocolate.txt
    new file mode 100644
    index 0000000..e69de29

MAHFUZUR RAHMAN@DESKTOP-4Q0OEE3 MINGW64 ~/Desktop/Devops/GitHub/Project-1 (master)


    MAHFUZUR RAHMAN@DESKTOP-4Q0OEE3 MINGW64 ~/Desktop/Devops/GitHub/Project-1 (master)
    $ git log --oneline
    ce7ce00 (HEAD -> master) Dark Chocolate added
    bf94956 Some chocolate added
    7367e81 ice cube added
    d361a8b Chocolate added
    5b41351 Two text file added

MAHFUZUR RAHMAN@DESKTOP-4Q0OEE3 MINGW64 ~/Desktop/Devops/GitHub/Project-1 (master)

    $ git diff bf94956 ce7ce00
    diff --git a/chocolate.txt b/chocolate.txt
    index 82f6c81..5c9e65f 100644
    --- a/chocolate.txt
    +++ b/chocolate.txt
    @@ -1 +1,3 @@
    -Some Chocolate added.
    \ No newline at end of file
    +Some Chocolate added.
    +
    +Dark Chocolate added.
    \ No newline at end of file

MAHFUZUR RAHMAN@DESKTOP-4Q0OEE3 MINGW64 ~/Desktop/Devops/GitHub/Project-1 (master)
$

MAHFUZUR RAHMAN@DESKTOP-4Q0OEE3 MINGW64 ~/Desktop/Devops/GitHub/Project-1 (master)

    $ git rm hot.txt
    rm 'hot.txt'

MAHFUZUR RAHMAN@DESKTOP-4Q0OEE3 MINGW64 ~/Desktop/Devops/GitHub/Project-1 (master)

    $ git status
    On branch master
    Changes to be committed:
      (use "git restore --staged <file>..." to unstage)
            modified:   chocolate.txt
            deleted:    hot.txt


MAHFUZUR RAHMAN@DESKTOP-4Q0OEE3 MINGW64 ~/Desktop/Devops/GitHub/Project-1 (master)

    $ git restore --staged hot.txt

MAHFUZUR RAHMAN@DESKTOP-4Q0OEE3 MINGW64 ~/Desktop/Devops/GitHub/Project-1 (master)

    $ git status
    On branch master
    Changes to be committed:
      (use "git restore --staged <file>..." to unstage)
            modified:   chocolate.txt

    Changes not staged for commit:
      (use "git add/rm <file>..." to update what will be committed)
      (use "git restore <file>..." to discard changes in working directory)
            deleted:    hot.txt


MAHFUZUR RAHMAN@DESKTOP-4Q0OEE3 MINGW64 ~/Desktop/Devops/GitHub/Project-1 (master)
$



MAHFUZUR RAHMAN@DESKTOP-4Q0OEE3 MINGW64 ~/Desktop/Devops/GitHub/Project-1 (master)

    $ git remote add origin https://github.com/dmahfuzd70/Practice

MAHFUZUR RAHMAN@DESKTOP-4Q0OEE3 MINGW64 ~/Desktop/Devops/GitHub/Project-1 (master)

    $ git push -u origin master
    To https://github.com/dmahfuzd70/Practice
     ! [rejected]        master -> master (fetch first)
    error: failed to push some refs to 'https://github.com/dmahfuzd70/Practice'
    hint: Updates were rejected because the remote contains work that you do
    hint: not have locally. This is usually caused by another repository pushing
    hint: to the same ref. You may want to first integrate the remote changes
    hint: (e.g., 'git pull ...') before pushing again.
    hint: See the 'Note about fast-forwards' in 'git push --help' for details.

MAHFUZUR RAHMAN@DESKTOP-4Q0OEE3 MINGW64 ~/Desktop/Devops/GitHub/Project-1 (master)

    $ git remote add origin https://github.com/dmahfuzd70/Practice.git
    fatal: remote origin already exists.


MAHFUZUR RAHMAN@DESKTOP-4Q0OEE3 MINGW64 ~/Desktop/Devops/GitHub/Project-1 (master)

    $ git push -u origin master -force
    error: did you mean `--force` (with two dashes)?

MAHFUZUR RAHMAN@DESKTOP-4Q0OEE3 MINGW64 ~/Desktop/Devops/GitHub/Project-1 (master)

    $ git push -u origin master --force
    Enumerating objects: 7, done.
    Counting objects: 100% (7/7), done.
    Delta compression using up to 4 threads
    Compressing objects: 100% (5/5), done.
    Writing objects: 100% (7/7), 677 bytes | 61.00 KiB/s, done.
    Total 7 (delta 0), reused 0 (delta 0), pack-reused 0
    To https://github.com/dmahfuzd70/Practice
     + 4e52d67...9261dad master -> master (forced update)
    Branch 'master' set up to track remote branch 'master' from 'origin'.

MAHFUZUR RAHMAN@DESKTOP-4Q0OEE3 MINGW64 ~/Desktop/Devops/GitHub/Project-1 (master)

