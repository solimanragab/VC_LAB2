![MyImage](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTOJ4IZbkwwyJD4dq7MObC7x1gpYN0xVkTOV_X9T9ZCMQ&s=10)
Git Questions & Answers

&#x20;Copy Markdown

The preview below uses Markdown formatting. No commands have been corrected.

## Q1: Create a new project on your local machine, then push it your remote repo.

```
git init
git add .
git commit -m “commit a”
git push -u origin main
```

## Q2: Create two branches (dev & test) then create one file on each branch, and push this changes to the remote repo.

```
git switch -c test
git add .
git commit -m “creating style.css in test branch”
git push origin test
```

```
git switch -c dev
git add .
git commit -m “creating main.js in dev branch”
git push origin dev
```

## Q3: Merge this changes on Main branch and then push it to your remote main branch.

```
git switch dev
git merge test

git switch main
git merge dev

git push origin main
```

## Q4: Tell me how to remove them locally and remotely.

locally:

```
git branch -d test
git branch -d dev
```

remotely:

```
git push origin –delete test
git push origin –delete dev
```

## Q5: Tell me how to checkout another branch without commit changes

```
git switch -c test2
git add .
“some changes “

git stash
git stash pop
```

## Q6: Create an annotated tag with tagname (v1.7).

```
git tag -a v1.0 -m "version 1.0"
```

## Q7: Push it to the remote repository.

```
git push origin v1.0
```

## Q8: Tell me how to list tags:

```
git tag
```

locally:

```
git tag --delete v1.0
```

remotely:

```
git push origin --delete v1.0
```
