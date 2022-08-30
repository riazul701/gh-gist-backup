# Gist Backup, Restore, Delete

## Installation
```shellscript
gh extension install riazul701/gh-gist-backup
```

## Do Work
* Login to GitHub before running extension commands (Choose HTTP protocol during login)
```shellscript
gh auth login
gh auth status
```

## Commands
* Backup Gist
```shellscript
gh gist-backup backup
```

* Restore Gist (Have to confirm 3 times)
```shellscript
gh gist-backup restore
```

* Delete Gist (Have to confirm 3 time)
```shellscript
gh gist-backup delete
```
