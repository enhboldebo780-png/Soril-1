My project
Git PR туршилт

User@216-11 MINGW64 ~
$ git clone https://github.com/enhboldebo780-png/Soril-1.git
Cloning into 'Soril-1'...
warning: You appear to have cloned an empty repository.

User@216-11 MINGW64 ~
$ cd Soril-1

User@216-11 MINGW64 ~/Soril-1 (main)
$ echo "My project" > README.md

User@216-11 MINGW64 ~/Soril-1 (main)
$ git add .
warning: in the working copy of 'README.md', LF will be replaced by CRLF the next time Git touches it

User@216-11 MINGW64 ~/Soril-1 (main)
$ git commit -m "Add readme"
[main (root-commit) 6490167] Add readme
 1 file changed, 1 insertion(+)
 create mode 100644 README.md

User@216-11 MINGW64 ~/Soril-1 (main)
$ git branch feature-test

User@216-11 MINGW64 ~/Soril-1 (main)
$ git checkout feature-test
Switched to branch 'feature-test'

User@216-11 MINGW64 ~/Soril-1 (feature-test)
$ code .

User@216-11 MINGW64 ~/Soril-1 (feature-test)
$ git add .
warning: in the working copy of 'README.md', LF will be replaced by CRLF the next time Git touches it

User@216-11 MINGW64 ~/Soril-1 (feature-test)
$ git commit -m "Add Feature-test"
[feature-test 8da2e72] Add Feature-test
 1 file changed, 1 insertion(+)

User@216-11 MINGW64 ~/Soril-1 (feature-test)
$ git push origin feature-test
Enumerating objects: 6, done.
Counting objects: 100% (6/6), done.
Delta compression using up to 20 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (6/6), 470 bytes | 470.00 KiB/s, done.
Total 6 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/enhboldebo780-png/Soril-1.git
 * [new branch]      feature-test -> feature-test

User@216-11 MINGW64 ~/Soril-1 (feature-test)
$ git checkout main
Switched to branch 'main'
Your branch is based on 'origin/main', but the upstream is gone.
  (use "git branch --unset-upstream" to fixup)

User@216-11 MINGW64 ~/Soril-1 (main)
$ git push
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
remote:
remote: Create a pull request for 'main' on GitHub by visiting:
remote:      https://github.com/enhboldebo780-png/Soril-1/pull/new/main
remote:
To https://github.com/enhboldebo780-png/Soril-1.git
 * [new branch]      main -> main

User@216-11 MINGW64 ~/Soril-1 (main)
$ git pull origin main
remote: Enumerating objects: 1, done.
remote: Counting objects: 100% (1/1), done.
remote: Total 1 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
Unpacking objects: 100% (1/1), 890 bytes | 445.00 KiB/s, done.
From https://github.com/enhboldebo780-png/Soril-1
 * branch            main       -> FETCH_HEAD
   6490167..c6e02d7  main       -> origin/main
Updating 6490167..c6e02d7
Fast-forward
 README.md | 1 +
 1 file changed, 1 insertion(+)

User@216-11 MINGW64 ~/Soril-1 (main)
$ git log --oneline
c6e02d7 (HEAD -> main, origin/main) Merge pull request #1 from enhboldebo780-png/feature-test
8da2e72 (origin/feature-test, feature-test) Add Feature-test
6490167 Add readme

User@216-11 MINGW64 ~/Soril-1 (main)
$
