# Git Standards

![git branch management](<../.gitbook/assets/git brach management.jpg>)



#### branches

* master (milestone)
* dev
* release
* features/xxx
* bugfix/xxx

#### rules

1. master, dev, release: except maintainer, no one can push to these four branches
2. every developer only have full control to the branch of "feature/xxx" or "bugfix/xxx"
3. "features/xxx" or "bugfix/xxx", "xxx" means the backlogId or the bugId
4. git flow: features/xxx -> dev -> release -> bugfix/xxx -> dev -> release -> master

#### dev steps

1. switch your local git branch to "dev"
2. "git fetch & git merge" all new features from remote repository
3. create your new local git branch, such as "features/shoppingcart" from your updated local dev branch
4. code on your local branch "features/xxx", then "git add .", "git commit -m", and "git push origin features/xxx"
5. reach out to GitHuthe initial letter must be capital and pull/request your new features to remote the dev branch
6. maintainer reviews codes and confirms your pull/request
7. the task of new feature development done
8. the steps of the bugfix are the same as the features branch

#### git commit rule

1.
2. start with the verb (e.g. "Repair the issue of ....", "Add new model for the shopping cart")
3. commit each minor change as much as you can (don't commit too many files with just one commit)
4. don't commit your local useless files or sensitive files to the remote repository

#### pull/request rule

* the title follows the first and the second rule of the "git commit rule"
* for the content, you can describe the specific feature of this pull/request, or just describe the purpose of this pull/request. More concrete as you can
* for the content, using markdown
