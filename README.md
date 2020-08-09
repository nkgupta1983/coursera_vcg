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

vi fileA.txt : add text again 
git add fileA.txt 
git commit -m "add​​ feature​​ 1"

Git checkout develop
git merge feature1

git push -u origin develop
