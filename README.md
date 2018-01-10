
[alias]
    amend = commit --amend
    st = status
    who = shortlog -sne
    oneline = log --pretty=oneline --abbrev-commit --graph
    changes = diff --name-status
    dic = diff --cached
    diffstat = diff --stat
    svnpull = svn rebase
    svnpush = svn dcommit
    lc = !git oneline ORIG_HEAD.. --stat --no-merges
    addm = !git-ls-files -m -z | xargs -0 git-add && git status
    addu = !git-ls-files -o --exclude-standard -z | xargs -0 git-add && git status
    rmm = !git ls-files -d -z | xargs -0 git-rm && git status
    mate = !git-ls-files -m -z | xargs -0 mate
    mateall = !git-ls-files -m -o --exclude-standard -z | xargs -0 mate
    undo = git reset --soft HEAD^
    amend = commit --amend
    changes = diff --name-status
    dic = diff --cached
    diffstat = diff --stat
    oneline = log --pretty=oneline --abbrev-commit --graph --decorate
    lc = !git oneline ORIG_HEAD.. --stat --no-merges
