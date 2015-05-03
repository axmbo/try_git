# try_git
try_git tutorial from Code School

Press enter to submit commands
 
> git init
 

Initialized empty Git repository in /.git/

Success!

$ git status
 

# On branch master
# Changes to be committed:
#   (use "git reset HEAD <file>..." to unstage)
#
#	new file:   octofamily/octodog.txt
#
# Changes not staged for commit:
#   (use "git add <file>..." to update what will be committed)
#   (use "git checkout -- <file>..." to discard changes in working directory)
#
#	modified:   octocat.txt
#

Use git diff to see what has changed

$ git diff --staged
 

diff --git a/octofamily/octodog.txt b/octofamily/octodog.txt
new file mode 100644
index 0000000..cfbc74a
--- /dev/null
+++ b/octofamily/octodog.txt
@@ -0,0 +1 @@
+[mwoof

Success!

$ git reset octofamily/octodog.txt
 


Success!

$ git checkout -- octocat.txt
 



Success!

$ git branch clean_up
 



Success!

$ git checkout clean_up
 

Switched to branch 'clean_up'

Success!

$ git rm '*.txt'
 

rm 'blue_octocat.txt'
rm 'octocat.txt'
rm 'octofamily/baby_octocat.txt'
rm 'octofamily/momma_octocat.txt'
rm 'red_octocat.txt'

Success!

$ git commit -m "Remove all the cats"
 

[clean_up 63540fe] Remove all the cats
 5 files changed, 5 deletions(-)
 delete mode 100644 blue_octocat.txt
 delete mode 100644 octocat.txt
 delete mode 100644 octofamily/baby_octocat.txt
 delete mode 100644 octofamily/momma_octocat.txt
 delete mode 100644 red_octocat.txt

Success!

$ git checkout master
 

Switched to branch 'master'

Success!

$ git merge clean_up
 

Updating 3852b4d..ec6888b
Fast-forward
 blue_octocat.txt             |    1 -
 octocat.txt                  |    1 -
 octofamily/baby_octocat.txt  |    1 -
 octofamily/momma_octocat.txt |    1 -
 red_octocat.txt              |    1 -
 5 files changed, 5 deletions(-)
 delete mode 100644 blue_octocat.txt
 delete mode 100644 octocat.txt
 delete mode 100644 octofamily/baby_octocat.txt
 delete mode 100644 octofamily/momma_octocat.txt
 delete mode 100644 red_octocat.txt

Success!

$ git branch -d clean_up
 

Deleted branch clean_up (was ec6888b).

Success!

$ git push
 

To https://github.com/try-git/try_git.git
   3e70b0f..c4c5241  master -> master

Success!

> 
