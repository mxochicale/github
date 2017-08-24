Useful Commands for [GitHub](https://en.wikipedia.org/wiki/GitHub)(2008)
---




# git clone


```
git clone https://github.com/...
```


# git push origin master

```
git add .  
git status  
git commit -m 'message'
git push origin master
```

# git pull

```
git pull
```


# pull-request


## Clone your fork to your local machine [ref](https://gist.github.com/Chaser324/ce0505fbed06b947d962#creating-a-fork)
```
git clone https://github.com/<myGitHubAccountName>/<repoName>.git
```

## Setting up Remotes
add your fork repo as a remote to your local cloned copy [ref1](https://stackoverflow.com/questions/14906187/how-to-submit-a-pull-request-from-a-cloned-repo)
[ref1](https://github.com/GarageGames/Torque2D/wiki/Cloning-the-repo-and-working-with-Git#3--setting-up-remotes)
```
git remote add YOUR_USER  https://github.com/<myGitHubAccountName>/<repoName>.git
```

## Managing-branches [ref](https://github.com/GarageGames/Torque2D/wiki/Cloning-the-repo-and-working-with-Git#4---managing-branches)

```
git branch newfeature # Create a new branch named newfeature(give your branch its own simple informative name)
git checkout newfeature # Switch to your new branch, making 'newfeature' our currently active branch

```



Finally, we target the most recent version of the repository that is linked to our
YOUR_USER remote(repoName) and pull in the contents of its "newfeature" branch into our currently active local branch.
[ref1](https://github.com/GarageGames/Torque2D/wiki/Cloning-the-repo-and-working-with-Git#4---managing-branches)
```
git pull YOUR_USER newfeature
```


## add files, commit changes and push it


to add all modified or new files in your entire project to your staging area.
```
git add .
```

Once your staging area is ready, you must commit your changes by typing
```
git commit -m 'hopefully relevant message about this commit'
```
[ref](https://github.com/GarageGames/Torque2D/wiki/Cloning-the-repo-and-working-with-Git#5---final-step--adding-files-committing-changes-and-pushing)


push the changes to your new remote
[ref2](https://hub.github.com/)
```
$ git push YOUR_USER newfeature
```



## pull a request
 Finally, go the github fage and a pull request for the topic branch you've just pushed





```
git checkout master #to return to your master branch,
```




# REFERENCES


[Well explained source for working with Git](https://github.com/GarageGames/Torque2D/wiki/Cloning-the-repo-and-working-with-Git)




# TODO

* Clean the previous explanaition
* Find a repository for data, this are some options:
[GHtorrent](http://ghtorrent.org/), [GitData](https://developer.github.com/v3/git/).


# Why I am using GitHub?

In 2013 at [INAOE Robotic's Lab](http://ccc.inaoep.mx/grupos/robotica.php),
I started my adventures with [GitHub](https://en.wikipedia.org/wiki/GitHub)
when I found the [GitHub of Jordan Frank](https://github.com/jwf/tdetools)
for which I started to learn a series of programming languages (e.g. R, C++, and GitHub). I am still learning, I think I have made a bit of advance. Anyway, but if you want to have more scientific evincence for the use of GitHub, the following paragraph summarise well, what GitHub is a super tool.

> "During recent years, [GitHub](https://en.wikipedia.org/wiki/GitHub),
founded in 2008, has become the largest code host in the world, with more
than 5M developers collaborating across 10M repositories.
Due to its support for distributed
version control (Git) and pull-based development [2], as well as
its modern Web UI and focus on social coding [ [4] ](http://www.jsntsay.com/publications/dabbish-cscw2012.pdf),
GITHUB has quickly surpassed
in size and popularity even much older forges such as Sourceforge (1999).
GITHUB offers a tremendous research potential. For instance, it is
a flagship for current open source development, a place for developers to
showcase their expertise to peers or potential recruiters, and
the platform where social coding features or pull requests emerged."
>
> [Gousios et al. 2014](https://bvasiles.github.io/papers/lean-ghtorrent.pdf)
