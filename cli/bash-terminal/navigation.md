# Navigation to the filesystem

#### Get the current directory

```bash
pwd
```

#### Get the contents of the current directory
```bash
ls

ls -la
# -a    Include directory entries whose names begin with a dot (.).
# -l    List in long format. 

ls -la ./a_sample_directory
# List files and directories inside `a_sample_directory`

```
> For more options like `-la` in  `ls -la` enter `man ls` to see all possible options you can use.


#### Changing directory
```bash

cd ~
# Brings you to your home directory


cd ..
# To go out in the parent directory of your current directory

cd ../the_sibling_of_your_current_directory
# To go out in the parent directory of your current directory and go to the specific directory inside your parent directory

cd /
# Brings you to your root direcotry


cd ~/Desktop
# An example of relative path starting from your Desktop

cd /var/www
# An example of navigation using absolute path


```


#### Going back to the last directory you were from
```
popd
```