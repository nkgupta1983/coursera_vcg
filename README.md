# coursera_vcg

create -> README.md

git checkout -b develop

vi fileA.txt
git add fileA.txt
git push -u origin develop

git checkout -b feature1
vi fileA.txt : add text 
git add fileA.txt 
git commit -m "feature​​ 1 ​​wip"

vi fileA.txt : edit text again 
git add fileA.txt 
git commit -m "add​​ feature​​ 1"

Git checkout develop
git merge feature1

git push -u origin develop

git checkout -b feature2
vi fileA.txt  -> edit text 
git add fileA.txt 
git commit -m "feature ​​2 ​​wip"
git push -u origin feature2

git checkout develop
git checkout -b release1
vi fileA.txt : edit text 
git add fileA.txt 
Git commit -m “release 1”
git push -u origin release1

Git checkout master
Git merge release1

git tag -a v1.00 -m "release1"
git push -u origin v1.00


git checkout release1
git checkout develop
git merge release1

git branch -d release1

git checkout feature2
git merge  master
vi fileA.txt -> resolve conflicts 
git add fileA.txt
git commit -m "feature​​ 2 ​​wip"
git push -u origin feature2

git checkout v1.00
git checkout -b hotfix1 
vi fileA.txt : edit text 
git add fileA.txt 
git commit -m "fix​​ feature​​ 1​​ bug​ ​Y"

git checkout master
Git merge hotfix1 : Or create pull request and merge to master 

git tag -a v1.01 -m "hotfix1"
Git push -u origin v1.01

Git checkout develop
Git merge hotfix1 : Or create pull request and merge to develop

Git branch -D hotfix1

git checkout feature2
git merge master
vi fileA.txt : resolve merge conflicts 
git add fileA.txt
git commit -m "feature​​ 2​​ wip"
git push -u origin feature2
