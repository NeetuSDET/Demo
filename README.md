
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


