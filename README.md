
(base) rajnishatrismbp:2026_Demo rajnishkhatri$ git config --global user.name
Neetu Khatri
(base) rajnishatrismbp:2026_Demo rajnishkhatri$ git config --global user.email
neeturk2@gmail.com
(base) rajnishatrismbp:2026_Demo rajnishkhatri$ git ls-remote origin
remote: Repository not found.
fatal: repository 'https://github.com/NeetuSDET/2026_Demo_Oct.git/' not found
(base) rajnishatrismbp:2026_Demo rajnishkhatri$ git ls-remote origin
remote: Repository not found.
fatal: repository 'https://github.com/NeetuSDET/2026_Demo_Oct.git/' not found
(base) rajnishatrismbp:2026_Demo rajnishkhatri$ git remote set-url origin https://github.com/NeetuSDET/Demo.git
(base) rajnishatrismbp:2026_Demo rajnishkhatri$ git remote -v
origin	https://github.com/NeetuSDET/Demo.git (fetch)
origin	https://github.com/NeetuSDET/Demo.git (push)
(base) rajnishatrismbp:2026_Demo rajnishkhatri$ git push -u origin main
To https://github.com/NeetuSDET/Demo.git
 ! [rejected]        main -> main (fetch first)
error: failed to push some refs to 'https://github.com/NeetuSDET/Demo.git'
hint: Updates were rejected because the remote contains work that you do not
hint: have locally. This is usually caused by another repository pushing to
hint: the same ref. If you want to integrate the remote changes, use
hint: 'git pull' before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.
(base) rajnishatrismbp:2026_Demo rajnishkhatri$ git push -u origin main --force
Enumerating objects: 24, done.
Counting objects: 100% (24/24), done.
Delta compression using up to 8 threads
Compressing objects: 100% (15/15), done.
Writing objects: 100% (24/24), 2.78 KiB | 2.78 MiB/s, done.
Total 24 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/NeetuSDET/Demo.git
 + 9c56328...052a75d main -> main (forced update)
branch 'main' set up to track 'origin/main'.
(base) rajnishatrismbp:2026_Demo rajnishkhatri$




Notes---- for pushing main to master

(base) rajnishatrismbp:2026_Demo rajnishkhatri$ git checkout -b master
Switched to a new branch 'master'
(base) rajnishatrismbp:2026_Demo rajnishkhatri$ git branch
  main
* master
(base) rajnishatrismbp:2026_Demo rajnishkhatri$ git push -u origin master
Enumerating objects: 24, done.
Counting objects: 100% (24/24), done.
Delta compression using up to 8 threads
Compressing objects: 100% (15/15), done.
Writing objects: 100% (24/24), 2.78 KiB | 1.39 MiB/s, done.
Total 24 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
remote: 
remote: Create a pull request for 'master' on GitHub by visiting:
remote:      https://github.com/NeetuSDET/Demo/pull/new/master
remote: 
To https://github.com/NeetuSDET/Demo.git
 * [new branch]      master -> master
branch 'master' set up to track 'origin/master'.
(base) rajnishatrismbp:2026_Demo rajnishkhatri$ git branch
  main
* master




Notes -- Added new file and updated project

git status
git add .
git status
git commit -m "Added new file and updated project"
git push origin master



Notes -- merge to main branch which i hv been modified in master
(
git status
git checkout main
git pull origin main
git merge master
esp 
:wq 
then we come for further command for terminal
git push origin main
)

(base) rajnishatrismbp:2026_Demo rajnishkhatri$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
(base) rajnishatrismbp:2026_Demo rajnishkhatri$ git branch
* main
  master
(base) rajnishatrismbp:2026_Demo rajnishkhatri$ git pull origin main
remote: Enumerating objects: 10, done.
remote: Counting objects: 100% (10/10), done.
remote: Compressing objects: 100% (9/9), done.
remote: Total 9 (delta 5), reused 0 (delta 0), pack-reused 0 (from 0)
Unpacking objects: 100% (9/9), 3.53 KiB | 516.00 KiB/s, done.
From https://github.com/NeetuSDET/Demo
 * branch            main       -> FETCH_HEAD
   052a75d..b968b68  main       -> origin/main
Updating 052a75d..b968b68
Fast-forward
 README.md | 76 ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 1 file changed, 76 insertions(+)
 create mode 100644 README.md
(base) rajnishatrismbp:2026_Demo rajnishkhatri$ git merge master
Merge made by the 'ort' strategy.
 src/test/java/Test/test1.java        |   4 +++-
 target/test-classes/Test/test1.class | Bin 518 -> 541 bytes
 2 files changed, 3 insertions(+), 1 deletion(-)
(base) rajnishatrismbp:2026_Demo rajnishkhatri$ git push origin main
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 8 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (2/2), 319 bytes | 319.00 KiB/s, done.
Total 2 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/NeetuSDET/Demo.git
   b968b68..37f01a5  main -> main
(base) rajnishatrismbp:2026_Demo rajnishkhatri$ git branch
* main
  master
(base) rajnishatrismbp:2026_Demo rajnishkhatri$ 

