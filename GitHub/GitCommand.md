## Git Initialization

    MAHFUZUR RAHMAN@DESKTOP-4Q0OEE3 MINGW64 ~/Desktop/Devops/GitHub/Project-1
    $ git init
    Initialized empty Git repository in C:/Users/MAHFUZUR RAHMAN/Desktop/Devops/GitHub/Project-1/.git/

## Set Username and Email

    MAHFUZUR RAHMAN@DESKTOP-4Q0OEE3 MINGW64 ~/Desktop/Devops/GitHub/Project-1 (master)
    $ git config --global user.name "Mahfuzur Rahman"

    MAHFUZUR RAHMAN@DESKTOP-4Q0OEE3 MINGW64 ~/Desktop/Devops/GitHub/Project-1 (master)

    $ git config --global user.email "dmahfuzd@gmail.com"

## Check User Information
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

## Create two file
    Mahfazur Rahman@MAHFUZ MINGW64 ~/Desktop/DevOps/GitHub (master)
    $ touch cold.txt hot.txt

## Check file
    Mahfazur Rahman@MAHFUZ MINGW64 ~/Desktop/DevOps/GitHub (master)
    $ ls
    cold.txt  hot.txtt

## Check Status(Unstage File)
    Mahfazur Rahman@MAHFUZ MINGW64 ~/Desktop/DevOps/GitHub (master)
    $ git status
    On branch master

    No commits yet

    Untracked files:
      (use "git add <file>..." to include in what will be committed)
            cold.txt
            hot.txt
    nothing added to commit but untracked files present (use "git add" to track)

## File Staging
    Mahfazur Rahman@MAHFUZ MINGW64 ~/Desktop/DevOps/GitHub (master)
    $ git add cold.txt
    
    Mahfazur Rahman@MAHFUZ MINGW64 ~/Desktop/DevOps/GitHub (master)
    $ git status
    On branch master

    No commits yet

    Changes to be committed:
      (use "git rm --cached <file>..." to unstage)
            new file:   cold.txt

    Untracked files:
      (use "git add <file>..." to include in what will be committed)
            hot.txt
    
    Mahfazur Rahman@MAHFUZ MINGW64 ~/Desktop/DevOps/GitHub (master)
    $ git add . 
    
    MAHFUZUR RAHMAN@DESKTOP-4Q0OEE3 MINGW64 ~/Desktop/Devops/GitHub/Project-1 (master)
    $ git add --all

    Mahfazur Rahman@MAHFUZ MINGW64 ~/Desktop/DevOps/GitHub (master)
    $ git status
    On branch master

    No commits yet

    Changes to be committed:
      (use "git rm --cached <file>..." to unstage)
            new file:   cold.txt
            new file:   hot.txt

## Git Commit
    Mahfazur Rahman@MAHFUZ MINGW64 ~/Desktop/DevOps/GitHub (master)
    $ git commit
    
    2 text file added
    # Please enter the commit message for your changes. Lines starting
    # with '#' will be ignored, and an empty message aborts the commit.
    #
    # On branch master
    #
    # Initial commit
    #
    # Changes to be committed:
    #       new file:   cold.txt
    #       new file:   hot.txt
    #
    ~
    ~
    ~
    ~
    ~

    Note: Open a file in editor mode
    
    [master (root-commit) ed2675a] 2 file added
    2 files changed, 0 insertions(+), 0 deletions(-)
    create mode 100644 cold.txt
    create mode 100644 hot.txt
     
    
    Mahfazur Rahman@MAHFUZ MINGW64 ~/Desktop/DevOps/GitHub (master)
    $ git status
    On branch master
    nothing to commit, working tree clean
    
    Mahfazur Rahman@MAHFUZ MINGW64 ~/Desktop/DevOps/GitHub (master)
    $ touch chocolate.txt
    
    $ git status
    On branch master
    Untracked files:
      (use "git add <file>..." to include in what will be committed)
            chocolate.txt
            
     Mahfazur Rahman@MAHFUZ MINGW64 ~/Desktop/DevOps/GitHub (master)
     $ git add .
     
     $ git commit -m "chocolate added"
    [master 74794d4] chocolate added
     1 file changed, 0 insertions(+), 0 deletions(-)
     create mode 100644 chocolate.txt
     
     $ git status
    On branch master
    nothing to commit, working tree clean

## To check commit status by git log command
    $ git log
    commit 74794d476ffd4ad25b3b701b7e5dfe1286c4ade4 (HEAD -> master)
    Author: Mahfuzur Rahman <dmahfuzd@gmail.com>
    Date:   Thu Jan 21 21:58:06 2021 +0600

        chocolate added

    commit ed2675aa48c6d39d537993489588fe888efa4d40
    Author: Mahfuzur Rahman <dmahfuzd@gmail.com>
    Date:   Thu Jan 21 21:53:00 2021 +0600

        2 file added
        
    $ git log --oneline
    74794d4 (HEAD -> master) chocolate added
    ed2675a 2 file added   

    Mahfazur Rahman@MAHFUZ MINGW64 ~/Desktop/DevOps/GitHub (master)
    $ echo "ice cube added" >> cold.txt
    
    $ git status
    On branch master
    Changes not staged for commit:
      (use "git add <file>..." to update what will be committed)
      (use "git restore <file>..." to discard changes in working directory)
            modified:   cold.txt

    no changes added to commit (use "git add" and/or "git commit -a")
    
    
    Mahfazur Rahman@MAHFUZ MINGW64 ~/Desktop/DevOps/GitHub (master)
    $ git add .
    
    Mahfazur Rahman@MAHFUZ MINGW64 ~/Desktop/DevOps/GitHub (master)
    $ git status
    On branch master
    Changes to be committed:
      (use "git restore --staged <file>..." to unstage)
            modified:   cold.txt
            
     Mahfazur Rahman@MAHFUZ MINGW64 ~/Desktop/DevOps/GitHub (master)
    $ git commit -m "ice cube added"
    [master 75a62a0] ice cube added
     1 file changed, 1 insertion(+)
     
    Mahfazur Rahman@MAHFUZ MINGW64 ~/Desktop/DevOps/GitHub (master)
    $ git status
    On branch master
    nothing to commit, working tree clean
    
    Mahfazur Rahman@MAHFUZ MINGW64 ~/Desktop/DevOps/GitHub (master)
    $ git log --oneline
    75a62a0 (HEAD -> master) ice cube added
    74794d4 chocolate added
    ed2675a 2 file added

## Back previous Stage by checkout command
    $ git checkout 74794d4
    Note: switching to '74794d4'.

    You are in 'detached HEAD' state. You can look around, make experimental
    changes and commit them, and you can discard any commits you make in this
    state without impacting any branches by switching back to a branch.

    If you want to create a new branch to retain commits you create, you may
    do so (now or later) by using -c with the switch command. Example:

      git switch -c <new-branch-name>

    Or undo this operation with:

      git switch -

    Turn off this advice by setting config variable advice.detachedHead to false

    HEAD is now at 74794d4 chocolate added
    
    Mahfazur Rahman@MAHFUZ MINGW64 ~/Desktop/DevOps/GitHub ((74794d4...))
    $ cat cold.txt

    Mahfazur Rahman@MAHFUZ MINGW64 ~/Desktop/DevOps/GitHub ((74794d4...))
    $ git log --oneline
    74794d4 (HEAD) chocolate added
    ed2675a 2 file added

    Mahfazur Rahman@MAHFUZ MINGW64 ~/Desktop/DevOps/GitHub ((74794d4...))
    $ git checkout ed2675a
    Previous HEAD position was 74794d4 chocolate added
    HEAD is now at ed2675a 2 file added
    
    Mahfazur Rahman@MAHFUZ MINGW64 ~/Desktop/DevOps/GitHub ((ed2675a...))
    $ ls
    cold.txt  hot.txt

    Mahfazur Rahman@MAHFUZ MINGW64 ~/Desktop/DevOps/GitHub ((ed2675a...))
    $ git checkout master
    Previous HEAD position was ed2675a 2 file added
    Switched to branch 'master'
    
    Mahfazur Rahman@MAHFUZ MINGW64 ~/Desktop/DevOps/GitHub (master)
    $ ls
    chocolate.txt  cold.txt  hot.txt
    
    Mahfazur Rahman@MAHFUZ MINGW64 ~/Desktop/DevOps/GitHub (master)
    $ cat cold.txt
    ice cube added
    
    
 ## To check latest change in last commit by git diff command
    Mahfazur Rahman@MAHFUZ MINGW64 ~/Desktop/DevOps/GitHub (master)
    $ ls
    chocolate.txt  cold.txt  hot.txt

    Mahfazur Rahman@MAHFUZ MINGW64 ~/Desktop/DevOps/GitHub (master)
    $ echo "some chocolate added" >> chocolate.txt

    Mahfazur Rahman@MAHFUZ MINGW64 ~/Desktop/DevOps/GitHub (master)
    $ cat chocolate.txt
    some chocolate added

    Mahfazur Rahman@MAHFUZ MINGW64 ~/Desktop/DevOps/GitHub (master)
    $ git status
    On branch master
    Changes not staged for commit:
      (use "git add <file>..." to update what will be committed)
      (use "git restore <file>..." to discard changes in working directory)
            modified:   chocolate.txt

    no changes added to commit (use "git add" and/or "git commit -a")
    
    Mahfazur Rahman@MAHFUZ MINGW64 ~/Desktop/DevOps/GitHub (master)
    $ git diff
    warning: LF will be replaced by CRLF in chocolate.txt.
    The file will have its original line endings in your working directory
    diff --git a/chocolate.txt b/chocolate.txt
    index e69de29..5ff6b14 100644
    --- a/chocolate.txt
    +++ b/chocolate.txt
    @@ -0,0 +1 @@
    +some chocolate added
    
    Mahfazur Rahman@MAHFUZ MINGW64 ~/Desktop/DevOps/GitHub (master)
    $ git log --oneline
    75a62a0 (HEAD -> master) ice cube added
    74794d4 chocolate added
    ed2675a 2 file added
    
    Mahfazur Rahman@MAHFUZ MINGW64 ~/Desktop/DevOps/GitHub (master)
    $ git show 74794d4
    commit 74794d476ffd4ad25b3b701b7e5dfe1286c4ade4
    Author: Mahfuzur Rahman <dmahfuzd@gmail.com>
    Date:   Thu Jan 21 21:58:06 2021 +0600

        chocolate added

    diff --git a/chocolate.txt b/chocolate.txt
    new file mode 100644
    index 0000000..e69de29
    
    Mahfazur Rahman@MAHFUZ MINGW64 ~/Desktop/DevOps/GitHub (master)
    $ git add .

    Mahfazur Rahman@MAHFUZ MINGW64 ~/Desktop/DevOps/GitHub (master)
    $ git commit -m "some chocolate added"
    [master 5123b9a] some chocolate added
     1 file changed, 1 insertion(+)
     
    5123b9a (HEAD -> master) some chocolate added
    75a62a0 ice cube added
    74794d4 chocolate added 
    ed2675a 2 file added
    
    Mahfazur Rahman@MAHFUZ MINGW64 ~/Desktop/DevOps/GitHub (master)
    $ echo "dark chocolate added" >> chocolate.txt

    Mahfazur Rahman@MAHFUZ MINGW64 ~/Desktop/DevOps/GitHub (master)
    $ cat chocolate.txt
    some chocolate added
    dark chocolate added
    
    Mahfazur Rahman@MAHFUZ MINGW64 ~/Desktop/DevOps/GitHub (master)
    $ git add .
    
    Mahfazur Rahman@MAHFUZ MINGW64 ~/Desktop/DevOps/GitHub (master)
    $ git commit -m "dark chocolate added"
    [master 34f3045] dark chocolate added
     1 file changed, 1 insertion(+)

    Mahfazur Rahman@MAHFUZ MINGW64 ~/Desktop/DevOps/GitHub (master)
    $ git log --oneline
    34f3045 (HEAD -> master) dark chocolate added
    5123b9a some chocolate added
    75a62a0 ice cube added
    74794d4 chocolate added
    ed2675a 2 file added
    
    Mahfazur Rahman@MAHFUZ MINGW64 ~/Desktop/DevOps/GitHub (master)
    $ git diff 5123b9a 34f3045
    diff --git a/chocolate.txt b/chocolate.txt
    index 5ff6b14..58d185c 100644
    --- a/chocolate.txt
    +++ b/chocolate.txt
    @@ -1 +1,2 @@
     some chocolate added
    +dark chocolate added
    
    Mahfazur Rahman@MAHFUZ MINGW64 ~/Desktop/DevOps/GitHub (master)
    $ echo "more chocolate added" >> chocolate.txt

    Mahfazur Rahman@MAHFUZ MINGW64 ~/Desktop/DevOps/GitHub (master)
    $ cat chocolate.txt
    some chocolate added
    dark chocolate added
    more chocolate added
    
    Mahfazur Rahman@MAHFUZ MINGW64 ~/Desktop/DevOps/GitHub (master)
    $ git status
    On branch master
    Changes not staged for commit:
      (use "git add <file>..." to update what will be committed)
      (use "git restore <file>..." to discard changes in working directory)
            modified:   chocolate.txt

    no changes added to commit (use "git add" and/or "git commit -a")
    
    Mahfazur Rahman@MAHFUZ MINGW64 ~/Desktop/DevOps/GitHub (master)
    $ git diff
    warning: LF will be replaced by CRLF in chocolate.txt.
    The file will have its original line endings in your working directory
    diff --git a/chocolate.txt b/chocolate.txt
    index 58d185c..2d15806 100644
    --- a/chocolate.txt
    +++ b/chocolate.txt
    @@ -1,2 +1,3 @@
     some chocolate added
     dark chocolate added
    +more chocolate added
    
    Mahfazur Rahman@MAHFUZ MINGW64 ~/Desktop/DevOps/GitHub (master)
    $ git add .

    Mahfazur Rahman@MAHFUZ MINGW64 ~/Desktop/DevOps/GitHub (master)
    $ git diff
    
    Mahfazur Rahman@MAHFUZ MINGW64 ~/Desktop/DevOps/GitHub (master)
    $ git diff --staged
    diff --git a/chocolate.txt b/chocolate.txt
    index 58d185c..2d15806 100644
    --- a/chocolate.txt
    +++ b/chocolate.txt
    @@ -1,2 +1,3 @@
     some chocolate added
     dark chocolate added
    +more chocolate added
    
    
 ## File delete
 
    Mahfazur Rahman@MAHFUZ MINGW64 ~/Desktop/DevOps/GitHub (master)
    $ git rm hot.txt
    rm 'hot.txt'

    Mahfazur Rahman@MAHFUZ MINGW64 ~/Desktop/DevOps/GitHub (master)
    $ git status
    On branch master
    Changes to be committed:
      (use "git restore --staged <file>..." to unstage)
            modified:   chocolate.txt
            deleted:    hot.txt


    Mahfazur Rahman@MAHFUZ MINGW64 ~/Desktop/DevOps/GitHub (master)
    $ git reset HEAD hot.txt
    Unstaged changes after reset:
    D       hot.txt

    Mahfazur Rahman@MAHFUZ MINGW64 ~/Desktop/DevOps/GitHub (master)
    $ git status
    On branch master
    Changes to be committed:
      (use "git restore --staged <file>..." to unstage)
            modified:   chocolate.txt

    Changes not staged for commit:
      (use "git add/rm <file>..." to update what will be committed)
      (use "git restore <file>..." to discard changes in working directory)
            deleted:    hot.txt
            
     Mahfazur Rahman@MAHFUZ MINGW64 ~/Desktop/DevOps/GitHub (master)
    $ git commit -m "hot text deleted"
    [master 20df374] hot text deleted
     1 file changed, 1 insertion(+)
     
 ## Local Repository connect with Remote Repository
     First create remote Repository in github.
     
     Mahfazur Rahman@MAHFUZ MINGW64 ~/Desktop/DevOps/GitHub (master)
     $ git remote add origin https://github.com/dmahfuzd70/Coffee.git
     
     Mahfazur Rahman@MAHFUZ MINGW64 ~/Desktop/DevOps/GitHub (master)
     $ git push -u origin master
     
     Note: Login prompt will be appear
     
     Enumerating objects: 17, done.
    Counting objects: 100% (17/17), done.
    Delta compression using up to 4 threads
    Compressing objects: 100% (13/13), done.
    Writing objects: 100% (17/17), 1.55 KiB | 317.00 KiB/s, done.
    Total 17 (delta 1), reused 0 (delta 0), pack-reused 0
    remote: Resolving deltas: 100% (1/1), done.
    To https://github.com/dmahfuzd70/Coffee.git
     * [new branch]      master -> master
    Branch 'master' set up to track remote branch 'master' from 'origin'.
    
    
 ## Local Repository connect with remote Repository by SSH Key
    Note: First remove login credential from windows to search credential in start bar search box.
    
    Make a directory name is git tuto then it initialize as a git directory
    
    Mahfazur Rahman@MAHFUZ MINGW64 ~/Desktop/GitHub
    $ git init
    Initialized empty Git repository in C:/Users/Mahfazur Rahman/Desktop/GitHub/.git/
    
    Mahfazur Rahman@MAHFUZ MINGW64 ~/Desktop/GitHub (master)
    $ touch student.txt
    
    Mahfazur Rahman@MAHFUZ MINGW64 ~/Desktop/GitHub (master)
    $ git status
    On branch master

    No commits yet

    Untracked files:
      (use "git add <file>..." to include in what will be committed)
            student.txt

    nothing added to commit but untracked files present (use "git add" to track)
    
    
    Mahfazur Rahman@MAHFUZ MINGW64 ~/Desktop/GitHub (master)
    $ git add .
    
    Mahfazur Rahman@MAHFUZ MINGW64 ~/Desktop/GitHub (master)
    $ git commit -m "commit student"
    [master (root-commit) c74747a] commit student
     1 file changed, 0 insertions(+), 0 deletions(-)
     create mode 100644 student.txt
     
     Mahfazur Rahman@MAHFUZ MINGW64 ~/Desktop/GitHub (master)
    $ ssh-keygen -t rsa -b 4096 -C "dmahfuzd@gmail.com"
    Generating public/private rsa key pair.
    Enter file in which to save the key (/c/Users/Mahfazur Rahman/.ssh/id_rsa):
    Enter passphrase (empty for no passphrase):
    Enter same passphrase again:
    Your identification has been saved in /c/Users/Mahfazur Rahman/.ssh/id_rsa
    Your public key has been saved in /c/Users/Mahfazur Rahman/.ssh/id_rsa.pub
    The key fingerprint is:
    SHA256:7draHMyNlnENa5Eh+74+JUcJ980tq7Fo6G+sNTghpx4 dmahfuzd@gmail.com
    The key's randomart image is:
    +---[RSA 4096]----+
    |          . .    |
    |           o.o.  |
    |          . +o +o|
    |         . . =+ =|
    |      . S o =..o |
    |       + * Oo +  |
    |      E oo@.oB   |
    |     . ..O=o+.   |
    |      ..=*=.o.   |
    +----[SHA256]-----+
    
    Mahfazur Rahman@MAHFUZ MINGW64 ~/Desktop/GitHub (master)
    $ eval $(ssh-agent -s)
    Agent pid 913
    
    Mahfazur Rahman@MAHFUZ MINGW64 ~/Desktop/GitHub (master)
    $ ssh-add ~/.ssh/id_rsa
    Identity added: /c/Users/Mahfazur Rahman/.ssh/id_rsa (dmahfuzd@gmail.com)
    
    Mahfazur Rahman@MAHFUZ MINGW64 ~/Desktop/GitHub (master)
    $ clip < ~/.ssh/id_rsa.pub
    
    Note: Copy public key for add with Remote Repository
    Go Remote Repository Setting > SSH and GPG Keys 
    
    Mahfazur Rahman@MAHFUZ MINGW64 ~/Desktop/GitHub (master)
    $ git remote add origin git@github.com:dmahfuzd70/git-tuto.git

    Mahfazur Rahman@MAHFUZ MINGW64 ~/Desktop/GitHub (master)
    $ git push -u origin master
    The authenticity of host 'github.com (52.74.223.119)' can't be established.
    RSA key fingerprint is SHA256:nThbg6kXUpJWGl7E1IGOCspRomTxdCARLviKw6E5SY8.
    Are you sure you want to continue connecting (yes/no/[fingerprint])? yes
    Warning: Permanently added 'github.com,52.74.223.119' (RSA) to the list of known hosts.
    Enumerating objects: 3, done.
    Counting objects: 100% (3/3), done.
    Writing objects: 100% (3/3), 219 bytes | 43.00 KiB/s, done.
    Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
    To github.com:dmahfuzd70/git-tuto.git
     * [new branch]      master -> master
    Branch 'master' set up to track remote branch 'master' from 'origin'.
    
    
    ## Download project from Remote Repository(clone, fetch, pull)
    
        
    
    
