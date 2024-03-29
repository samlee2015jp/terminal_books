# mac setup

https://sourabhbajaj.com/mac-setup/


# Using Homebrew

To install a package (or Formula in Homebrew vocabulary) simply type:

brew install <formula>
To update Homebrew's directory of formulae, run:

brew update
Note: If that command fails you can manually download the directory of formulas like this:

cd /usr/local/Homebrew/
git fetch origin
git reset --hard origin/master
To see if any of your formulas need to be updated:

brew outdated
To update a formula:

brew upgrade <formula>
Homebrew keeps older versions of formulas installed on your system, in case you want to roll back to an older version. That is rarely necessary, so you can do some cleanup to get rid of those old versions:

brew cleanup
If you want to see what formulae Homebrew would delete without actually deleting them, you can run:

brew cleanup --dry-run
To see what you have installed (with their version numbers):

brew list --versions
To search for formulas you run:

brew search <formula>
To get more information about a formula you run:

brew info <formula>
To uninstall a formula you can run:

brew uninstall <formula>
  
# git
```
git config --global credential.helper osxkeychain
```
  
If you are setting up a new repo, add at least one file and commit first. Then, configure the remote and push to GitHub by running:

```
git remote add origin https://github.com/<username>/<repo-name>.git
git push -u origin master
  
git config --global core.excludesfile ~/.gitignore
```

# terminal
learning terminal

http://swcarpentry.github.io/shell-novice/

### show root directory

```
sudo chflags nohidden /usr
```

Reverse this by typing:
```
sudo chflags hidden /usr
```
remove the protection
```
csrutil disable
```
reverse the action above
```
csrutil enable
```
