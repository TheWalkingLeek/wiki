**branchX = branch to merge into master**

* git co branchX
* git rebase master
* {fix conflicts}
* {run tests}
* git st
* git co master
* git merge --no-commit branchX
* gitg
* {run tests}
* git st
* git push origin master