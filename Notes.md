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
	- `--stat`: show change statistics
	- `--pretty={format}`: change log output format

## author: originally wrore the work
## committer: person who last applied the work

### `git log --since=2.weeks`: limit log output by time
### `git log -S {string}`: show only commits that changed the number of occurrences of {string}
### `git commit --ammend`: edit most recent commit
####	useful for adding forgotten files or changing commit message
####	ONLY ammend local commits, not pushed commits
### `git reset HEAD file.name`: unstage file.name
### `git restore --staged file.name`: ^
### `git remote add <shortname> <url>`: add new remote git repository
### `git pull`: fetch + merge
### `git push <remote> <branch>`
