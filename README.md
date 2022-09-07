# Gist Backup, Restore, Delete

## Installation

```shellscript
gh extension install riazul701/gh-gist-backup
```

## Uninstallation

```shellscript
gh extension remove gist-backup
```

## Do Work

* Login to GitHub before running extension commands (Choose HTTP protocol during login)
```shellscript
gh auth login
gh auth status
```

* To Logout from GitHub CLI enter command
```shellscript
gh auth logout
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

## NOTE

* Windows is Case-Insensitive OS and Linux (Ubuntu) OS is Case-Sensitive OS. If any gist contains two files named "abc.php" and "Abc.php", then only one file will be downloaded in Windows OS and both file will be downloaded in Linux (Ubuntu) OS. So it is recommended to use Linux (Ubuntu) OS for backing up gists.

* If "Gist_Backup.zip" file contains two files named "abc.php" and "Abc.php" and we try to unzip the backup zip file in Windows OS, then one file will be replaced by another because Windows is Case-Insensitive OS. So it is recommended to use Linux (Ubuntu) OS for unzipping the backup zip file.

## Troubleshooting

* **Problem 1: Extension run error**

> **Problem:** After installing extension by command `gh extension install riazul701/gh-gist-backup`, when running gist-backup command `gh gist-backup backup`, then this error shows:
>> failed to run extension: fork/exec /home/<user_name>/.local/share/gh/extensions/gh-gist-backup/gh-gist-backup: permission denied
>
> **Solution:** 
> * Open folder "/home/<user_name>/.local/share/gh/extensions/gh-gist-backup/"
> * Right click on file "gh-gist-backup" -> Properties -> Permissions -> Select "Execute: Anyone"

## Website Link

* [GitHub CLI](https://cli.github.com/)