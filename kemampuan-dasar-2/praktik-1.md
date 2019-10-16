# kemampuan-dasar-2
Microsoft Windows [Version 10.0.17134.950]
(c) 2018 Microsoft Corporation. All rights reserved.

C:\Users\HP>mkdir rhymes

C:\Users\HP>cd rhymes

C:\Users\HP\rhymes>git init
Initialized empty Git repository in C:/Users/HP/rhymes/.git/

HP@LAPTOP-660E9LSI MINGW64 ~/rhymes (master)
$ touch README.txt

HP@LAPTOP-660E9LSI MINGW64 ~/rhymes (master)
$ git add README.txt

HP@LAPTOP-660E9LSI MINGW64 ~/rhymes (master)
$ git commit -m 'First commit'
[master (root-commit) 02f4006] First commit
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 README.txt

HP@LAPTOP-660E9LSI MINGW64 ~/rhymes (master)
$ echo 'This repo is a collection of my favorite nursery rhymes.' >> README.txt

HP@LAPTOP-660E9LSI MINGW64 ~/rhymes (master)
$ git status
On branch master
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.txt

no changes added to commit (use "git add" and/or "git commit -a")

HP@LAPTOP-660E9LSI MINGW64 ~/rhymes (master)
$ git diff
warning: LF will be replaced by CRLF in README.txt.
The file will have its original line endings in your working directory
diff --git a/README.txt b/README.txt
index e69de29..c83e022 100644
--- a/README.txt
+++ b/README.txt
@@ -0,0 +1 @@
+This repo is a collection of my favorite nursery rhymes.

HP@LAPTOP-660E9LSI MINGW64 ~/rhymes (master)
$ git add README.txt
warning: LF will be replaced by CRLF in README.txt.
The file will have its original line endings in your working directory

HP@LAPTOP-660E9LSI MINGW64 ~/rhymes (master)
$ git commit -m 'Added project overview to README.txt'
[master 610ca97] Added project overview to README.txt
 1 file changed, 1 insertion(+)
 
 HP@LAPTOP-660E9LSI MINGW64 ~/rhymes (master)
$ git add .
warning: LF will be replaced by CRLF in rhymes-master/README.txt.
The file will have its original line endings in your working directory
warning: LF will be replaced by CRLF in rhymes-master/all-around-the-mulberry-bush.txt.
The file will have its original line endings in your working directory
warning: LF will be replaced by CRLF in rhymes-master/hickory-dickory-dock.txt.
The file will have its original line endings in your working directory
warning: LF will be replaced by CRLF in rhymes-master/hokey-pokey.txt.
The file will have its original line endings in your working directory
warning: LF will be replaced by CRLF in rhymes-master/jack-and-jill.txt.
The file will have its original line endings in your working directory
warning: LF will be replaced by CRLF in rhymes-master/old-mother-hubbard.txt.
The file will have its original line endings in your working directory
warning: LF will be replaced by CRLF in rhymes-master/roses-are-red.txt.
The file will have its original line endings in your working directory
warning: LF will be replaced by CRLF in rhymes-master/twinkle-twinkle.txt.
The file will have its original line endings in your working directory

HP@LAPTOP-660E9LSI MINGW64 ~/rhymes (master)
$ git commit -m 'Added old-mother-hubbard.txt, twinkle-twinkle.txt, hokey-pokey.tx
t'
[master fbf8ddf] Added old-mother-hubbard.txt, twinkle-twinkle.txt, hokey-pokey.txt
 8 files changed, 101 insertions(+)
 create mode 100644 rhymes-master/README.txt
 create mode 100644 rhymes-master/all-around-the-mulberry-bush.txt
 create mode 100644 rhymes-master/hickory-dickory-dock.txt
 create mode 100644 rhymes-master/hokey-pokey.txt
 create mode 100644 rhymes-master/jack-and-jill.txt
 create mode 100644 rhymes-master/old-mother-hubbard.txt
 create mode 100644 rhymes-master/roses-are-red.txt
 create mode 100644 rhymes-master/twinkle-twinkle.txt
 
 HP@LAPTOP-660E9LSI MINGW64 ~/rhymes (master)
$ git log
commit fbf8ddfb2c84f263ea38a20b65fecef4e768b322 (HEAD -> master)
Author: nrfitriani <54707827+nrfitriani@users.noreply.github.com>
Date:   Wed Oct 16 19:28:39 2019 +0800

    Added old-mother-hubbard.txt, twinkle-twinkle.txt, hokey-pokey.txt

commit 610ca970ef44f9186d2f7fe8078dbcfc3c49d54e
Author: nrfitriani <54707827+nrfitriani@users.noreply.github.com>
Date:   Wed Oct 16 19:23:01 2019 +0800

    Added project overview to README.txt

commit 02f4006fcc21442244087cd3c538573ec9ef8713
Author: nrfitriani <54707827+nrfitriani@users.noreply.github.com>
Date:   Wed Oct 16 19:21:44 2019 +0800

    First commit
    
    HP@LAPTOP-660E9LSI MINGW64 ~/rhymes (master)
$ git log
commit fbf8ddfb2c84f263ea38a20b65fecef4e768b322 (HEAD -> master)
Author: nrfitriani <54707827+nrfitriani@users.noreply.github.com>
Date:   Wed Oct 16 19:28:39 2019 +0800

    Added old-mother-hubbard.txt, twinkle-twinkle.txt, hokey-pokey.txt

commit 610ca970ef44f9186d2f7fe8078dbcfc3c49d54e
Author: nrfitriani <54707827+nrfitriani@users.noreply.github.com>
Date:   Wed Oct 16 19:23:01 2019 +0800

    Added project overview to README.txt

commit 02f4006fcc21442244087cd3c538573ec9ef8713
Author: nrfitriani <54707827+nrfitriani@users.noreply.github.com>
Date:   Wed Oct 16 19:21:44 2019 +0800

    First commit

HP@LAPTOP-660E9LSI MINGW64 ~/rhymes (master)
$ git log --oneline
fbf8ddf (HEAD -> master) Added old-mother-hubbard.txt, twinkle-twinkle.txt, hokey-pokey.txt
610ca97 Added project overview to README.txt
02f4006 First commit

HP@LAPTOP-660E9LSI MINGW64 ~/rhymes (master)
$ git log -p
commit fbf8ddfb2c84f263ea38a20b65fecef4e768b322 (HEAD -> master)
Author: nrfitriani <54707827+nrfitriani@users.noreply.github.com>
Date:   Wed Oct 16 19:28:39 2019 +0800

    Added old-mother-hubbard.txt, twinkle-twinkle.txt, hokey-pokey.txt

diff --git a/rhymes-master/README.txt b/rhymes-master/README.txt
new file mode 100644
index 0000000..c83e022
--- /dev/null
+++ b/rhymes-master/README.txt
@@ -0,0 +1 @@
+This repo is a collection of my favorite nursery rhymes.
diff --git a/rhymes-master/all-around-the-mulberry-bush.txt b/rhymes-master/all-around-the-mulberry-bush.txt
new file mode 100644
index 0000000..b77d989
--- /dev/null
+++ b/rhymes-master/all-around-the-mulberry-bush.txt
@@ -0,0 +1,19 @@
+All around the mulberry bush
+The monkey chased the weasel.
+The monkey thought 'twas all in fun.
+Pop! goes the weasel.
+
+A penny for a spool of thread,
+A penny for a needle.
+That's the way the money goes.
+Pop! goes the weasel.

$ git log -p
commit fbf8ddfb2c84f263ea38a20b65fecef4e768b322 (HEAD -> master)
Author: nrfitriani <54707827+nrfitriani@users.noreply.github.com>
Date:   Wed Oct 16 19:28:39 2019 +0800

    Added old-mother-hubbard.txt, twinkle-twinkle.txt, hokey-pokey.txt

diff --git a/rhymes-master/README.txt b/rhymes-master/README.txt
new file mode 100644
index 0000000..c83e022
--- /dev/null
+++ b/rhymes-master/README.txt
@@ -0,0 +1 @@
+This repo is a collection of my favorite nursery rhymes.
diff --git a/rhymes-master/all-around-the-mulberry-bush.txt b/rhymes-master/all-around-the-mulberry-bush.txt
new file mode 100644
index 0000000..b77d989
--- /dev/null
+++ b/rhymes-master/all-around-the-mulberry-bush.txt
@@ -0,0 +1,19 @@
+All around the mulberry bush
+The monkey chased the weasel.
+The monkey thought 'twas all in fun.
+Pop! goes the weasel.
+
+A penny for a spool of thread,
+A penny for a needle.
+That's the way the money goes.
+Pop! goes the weasel.
+
+Up and down the City Road,
+In and out of the Eagle,
+That's the way the money goes.
+Pop! goes the weasel.
+
+Half a pound of tuppenney rice,
+Half a pound of treacle,
+Mix it up and make it nice,
+Pop! goes the weasel.
diff --git a/rhymes-master/hickory-dickory-dock.txt b/rhymes-master/hickory-dickory-dock.txt
new file mode 100644
index 0000000..a337f4c
--- /dev/null
+++ b/rhymes-master/hickory-dickory-dock.txt
@@ -0,0 +1,5 @@
+Hickory, dickory, dock,
+The mouse ran up the clock.
+The clock struck one,
+The mouse ran down!
+Hickory, dickory, dock.
diff --git a/rhymes-master/hokey-pokey.txt b/rhymes-master/hokey-pokey.txt
new file mode 100644
index 0000000..97f425b
--- /dev/null
+++ b/rhymes-master/hokey-pokey.txt
@@ -0,0 +1,16 @@
+You put your right foot in,
+You put your right foot out;
+You put your right foot in,
+And you shake it all about.
+You do the Hokey-Pokey,
+And you turn yourself around.
+That's what it's all about!
+
+You put your left foot in...
+You put your right hand in...
+You put your right side in...
+You put your nose in...
+You put your tail in...
+You put your head in...
+You put your whole self in...
+
diff --git a/rhymes-master/jack-and-jill.txt b/rhymes-master/jack-and-jill.txt
new file mode 100644
index 0000000..1596bce
--- /dev/null
+++ b/rhymes-master/jack-and-jill.txt
@@ -0,0 +1,12 @@
+Jack and Jill
+Went up the hill
+To fetch a pail of water.
+Jack fell down
+And broke his crown
+And Jill came tumbling after.
+Up Jack got
+And home did trot
+As fast as he could caper
+Went to bed
+And plastered his head
+With vinegar and brown paper.
diff --git a/rhymes-master/old-mother-hubbard.txt b/rhymes-master/old-mother-hubbard.txt
new file mode 100644
index 0000000..c91ff71
--- /dev/null
+++ b/rhymes-master/old-mother-hubbard.txt
@@ -0,0 +1,34 @@
+Old Mother Hubbard
+Went to the cupboard
+To fetch her poor dog a bone;
+But when she came there
+The cupboard was bare,
+And so the poor dog had none.
+She took a clean dish
+To get him some tripe;
+But when she came back
+He was smoking a pipe.
+She went to the grocer's
+To buy him some fruit;
+But when she came back
+He was playing the flute.
+
+She went to the baker's
+To buy him some bread;
+But when she came back
+The poor dog was dead.
+
+She went to the undertaker's
+To buy him a coffin;
+But when she came back
+The poor dog was laughing.
+
+She went to the hatter's
+To buy him a hat;
+But when she came back
+He was feeding the cat.
+
+The dame made a curtsey,
+The dog made a bow;
+The dame said, "Your servant."
+The dog said, "Bow wow!"
diff --git a/rhymes-master/roses-are-red.txt b/rhymes-master/roses-are-red.txt
new file mode 100644
index 0000000..efba165
--- /dev/null
+++ b/rhymes-master/roses-are-red.txt
@@ -0,0 +1,8 @@
+Roses are red
+-------------
+
+Roses are red
+Violets are blue
+Nobody loves GitHub
+More than government agencies do!
+
diff --git a/rhymes-master/twinkle-twinkle.txt b/rhymes-master/twinkle-twinkle.txt

HP@LAPTOP-660E9LSI MINGW64 ~/rhymes (master)
$ git remote add origin https://github.com/nrfitriani/rhymes.git

HP@LAPTOP-660E9LSI MINGW64 ~/rhymes (master)
$ git push -u origin master
Enumerating objects: 16, done.
Counting objects: 100% (16/16), done.
Delta compression using up to 8 threads
Compressing objects: 100% (13/13), done.
Writing objects: 100% (16/16), 2.19 KiB | 560.00 KiB/s, done.
Total 16 (delta 1), reused 0 (delta 0)
remote: Resolving deltas: 100% (1/1), done.
To https://github.com/nrfitriani/rhymes.git
 * [new branch]      master -> master
Branch 'master' set up to track remote branch 'master' from 'origin'.
new file mode 100644
index 0000000..5585462
--- /dev/null
+++ b/rhymes-master/twinkle-twinkle.txt
@@ -0,0 +1,6 @@
+Twinkle, twinkle, little star,
+How I wonder what you are.
+Up above the world so high,
+Like a diamond in the sky.
+Twinkle, twinkle, little star,
+How I wonder what you are.

commit 610ca970ef44f9186d2f7fe8078dbcfc3c49d54e
Author: nrfitriani <54707827+nrfitriani@users.noreply.github.com>
Date:   Wed Oct 16 19:23:01 2019 +0800

    Added project overview to README.txt

diff --git a/README.txt b/README.txt
index e69de29..c83e022 100644
--- a/README.txt
+++ b/README.txt
@@ -0,0 +1 @@
+This repo is a collection of my favorite nursery rhymes.

commit 02f4006fcc21442244087cd3c538573ec9ef8713
Author: nrfitriani <54707827+nrfitriani@users.noreply.github.com>
Date:   Wed Oct 16 19:21:44 2019 +0800

    First commit

diff --git a/README.txt b/README.txt
new file mode 100644
index 0000000..e69de29
