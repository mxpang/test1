git is a distributed version control system.
git is free software

- initialize a git
    git init
- add files to git repository
    git add <file1> <file2> <file3>...<filen>
- commit
    git commit -m "some_intro"

- check status
    git status

- check differences
    git diff

- check modification logs
    git log
    git log --pretty=oneline   #format output line by line
- roll back to a specifed version
    首先，Git必须知道当前版本是哪个版本，在Git中，用HEAD表示当前版本，也就是最新的提交3628164...882e1e0（注意我的提交ID和你的肯定不一样），上一个版本就是HEAD^，上上一个版本就是HEAD^^，当然往上100个版本写100个^比较容易数不过来，所以写成HEAD~100
    1. get the commit id in the command window
    2. git reset --hard <commit_id>
    2. git reset --hard HEAD^ #roll back to the previous version
    