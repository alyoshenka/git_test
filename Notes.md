## change name of default branch
###	git config --global init.defaultBranch {name}

## list all git settings
###	git config --list

## glob patterns
- * : 0+ characters
- [abc] : any character inside brackets
- ? : single character
- [0-9] : any charachter within bracket rande
- a/**/z : nested directories

## git diff shows only unstaged changes
## be sure to use `git rm` instead of `rm` to remove files
###	use `--cached` to remove from staging area

## `git log`: see commit history
	- `-p`: changes
	- `-{num}`: most recent {num} entries
