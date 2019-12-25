###### Branch

* > * **master**
  >
  > * **dev**
  >
  > * **release / staging**

#### Creating a feature branch {#creating-a-feature-branch}

```
git checkout -b myfeature dev
```

####  {#incorporating-a-finished-feature-on-develop}

#### Incorporating a finished feature on develop {#incorporating-a-finished-feature-on-develop}

Switched to branch 'dev'

```
git checkout dev
```

Summary of changes

```
git merge --no-ff my_feature
```

Deleted branch my\_feature

```
git branch -d my_feature
```

Push

```
git push origin develop
```

![](/assets/Screen Shot 2019-12-25 at 15.33.33.png)

#### Creating a release branch {#creating-a-release-branch}

```
git checkout -b release-1.2 develop
```

####  {#finishing-a-release-branch}

#### Finishing a release branch {#finishing-a-release-branch}

```
git checkout master
```

```
git merge --no-ff release-1.2
```

```
git tag v1.2
```

```
git branch -d release-1.2
```



