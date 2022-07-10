---
title: Gives commit history
tags: log,commit,repository
expertise: intermediate
firstSeen: 2022-07-10T07:09:33+0000
---

Gives log history of commits in the repository.

- Use `git log` to see all commit history in the current reposity.
- It displays details as `secure hash algorithim(SHA)`, `author`, `date` and `commit message`.
- Use `git log --oneline` to see commit history in one line and short form, it displays `one commit per line` with `first seven characters of SHA` and `commit message`.
- Use `git log --graph` to view git log in graph representation form, this can also be combined with `--oneline` flag.
- Use `git log --stat` to see files modified in each commit and lines added or removed. 
- Use `git log --patch` or `git log -p` to see files modifed, added, removed or changed by you.

```shell
git log
```

```shell
git log --oneline
# 0e25143 Merge branch 'feature'
# ad8621a Fix a bug in the feature
```

```shell
git log --graph
```

```shell
git log --graph --oneline
#* 0e25143 (HEAD, main) Merge branch 'feature'
#|\  
#| * 16b36c6 Fix a bug in the new feature
#* | ad8621a Fix a critical security issue
#|/  
#* 400e4b7 Fix typos in the documentation
```

```shell
git log --stat
#commit f2a238924e89ca1d4947662928218a06d39068c3
#Author: john <john@gmail.com>
#Date:   Fri Jun 25 17:30:28 2022 -0500

#    Add a new feature

# hello.js | 105 ++++++++++++++++++++++++-----------------
# 1 file changed, 67 insertion(+), 38 deletions(-)
```

```shell
git log --patch
```