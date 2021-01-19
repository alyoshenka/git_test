`author`: originally wrote the work

`committer`: person who last applied the work

In “detached HEAD” state, if you make changes and then create a commit, the tag will stay the same,
but your new commit won’t belong to any branch and will be unreachable, except by the exact
commit hash. Thus, if you need to make changes — say you’re fixing a bug on an older version, for
instance — you will generally want to create a branch

*Do not rebase commits that exist outside your reposityry and that people may have based work on*

Rebasing replays changes from one line of woek onto another in the order they were introduced, whereas merging rakes the endpoints and merges them together

`git log` will by default only shoe commit history below the branch you've checked out

run `git status` to see which files are unmerged at any point after a merge conflict

`remote tracking branch`: reference to the state of a remote branch

`tracking branch`: local branch that has a direct relationship to a remote branch

`@{u/upstream}`: reference a branch's upstream branch

glob patterns
- `\*` : 0+ characters
- `[abc]` : any character inside brackets
- `?` : single character
- `[0-9]` : any charachter within bracket rande
- `a/**/z` : nested directories

git diff shows only unstaged changes
- be sure to use `git rm` instead of `rm` to remove files
- use `--cached` to remove from staging area

`git log`: see commit history
- `-p`: changes
- `-{num}`: most recent {num} entries
- `--stat`: show change statistics
- `--pretty={format}`: change log output format

`git config --global init.defaultBranch {name}`: change name of default branch

`git config --list`: list all git settings

`git log --since=2.weeks`: limit log output by time

`git log -S {string}`: show only commits that changed the number of occurrences of {string}

`git commit --ammend`: edit most recent commit
- useful for adding forgotten files or changing commit message
- ONLY ammend local commits, not pushed commits
	
`git reset HEAD file.name`: unstage file.name

`git restore --staged file.name`: ^

`git remote add <shortname> <url>`: add new remote git repository

`git pull`: fetch + merge

`git push <remote> <branch>`

`git tag (-l)`: list existing tags
- `lightweight`: just a pointer to a specific commit
- `annotated`: full object, checksummed, contains tagger info

`git tag -a {version #} -m "tag annotation"`

`git show {version #}`: view tag data

`git push origin <tagname>`: push tag to remote

`git config alias.{cmd} "long command"`

`HEAD`: pointer to the local branch you're currently on

`git branch --merged`: branches merged into current branch

`git clone -o "origin name"`: clone repository with "origin name" as wrigin name

`git push origin <localbranchname>:<remotebranchname>`

`git config --global credential.helper cache`: set up credential cache
