# Git - Config

#### Setting your name & email globally

``` bash
git config --global user.name "Your Name Here"

git config --global user.email "Your Email Here"
```

> By setting `--global` means git will use these configuration by default on git repositories you initiate on your system. 


### Setting your name & email in your local git repoistory directory

``` bash
git config user.name "Your Name Here"

git config user.email "Your Email Here"
```


### Checking if your config has taken effect

``` bash
git config user.name
# The code above will return the name you've set

git config user.email
# The code above will return the email you've set
```