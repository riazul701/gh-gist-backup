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

## Troubleshooting

* **Problem 1: Extension run error**

> **Problem:** After installing extension by command `gh extension install riazul701/gh-gist-backup`, when running gist-backup command `gh gist-backup backup`, then this error shows:
>> failed to run extension: fork/exec /home/<user_name>/.local/share/gh/extensions/gh-gist-backup/gh-gist-backup: permission denied
>
> **Solution:** 
> * Open folder "/home/<user_name>/.local/share/gh/extensions/gh-gist-backup/"
> * Right click on file "gh-gist-backup" -> Properties -> Permissions -> Select "Execute: Anyone"

