# Modifying files and directories

#### Deleting dot files:

```bash
rm -rf .[!.]* ..?*
```

```zsh
find . -name . -o -prune -exec rm -rf -- {} +
```


#### Recursively set the permission of files and directories

```bash
find . -type d -exec chmod 775 {} \;
find . -type f -exec chmod 664 {} \;
```
