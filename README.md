![MyImage](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTOJ4IZbkwwyJD4dq7MObC7x1gpYN0xVkTOV_X9T9ZCMQ&s=10)


Q1:Create a new project on your local machine,
then push it your remote repo.

git init <br>
git add .<br>
git commit -m “commit a”<br>
git push -u origin main<br>

Q2:Create two branches (dev & test) then create one
file on each branch, and push this changes to the remote repo.
<br>
git switch -c test<br>
git add .<br>

git commit -m “creating style.css in test branch”<br>

git push origin test<br>
<br>
git switch -c dev
<br>
git add .
<br>
git commit -m “creating main.js in dev branch”
<br>
git push origin dev
<br>
Q3:Merge this changes on Main branch and then push it to your
remote main branch.
<br>

git switch dev<br>
git merge test<br>

git switch main<br>
git merge dev<br>

git push origin main<br>

Q4:Tell me how to remove them locally and remotely.<br>

locally:<br>
git branch -d  test<br>
git branch -d dev<br>

remotely: <br>
git push origin –delete test<br> 
git push origin –delete dev<br>
<br>
Q5:Tell me how to checkout another branch without commit
changes
<br>
git switch -c test2<br>
git add .<br>
“some changes “<br>

git stash <br>
git stash pop<br>

Q6: Create an annotated tag with tagname (v1.7) .<br>

git tag -a v1.0 -m "version 1.0"<br>

Q7:Push it to the remote repository.<br>
git push origin v1.0<br>

Q8:Tell me how to list tags:<br>

git tag<br>

locally:<br>
git tag --delete v1.0<br>
remotely:<br>
git push origin --delete v1.0<br>


