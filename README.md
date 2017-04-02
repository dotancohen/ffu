# uu

CLI script for uploading code and performing other common operations on a remote server



## Description

`uu` is used to easily upload code, access SSH, and access a remote database on remote servers. It supports both FTP and SCP methods of code upload, and of course supports the use of public/private keys for connecting via SSH. It searches each successive parent directory for a `.uu` configuration file, allowing one to use it in any project directory. The `.uu` confige file should not be added to Git or other version control system as it is likely to contain sensitive information.



# Using uu

## Confige uu
```
$ vim .uu
```

## Instruct Git to ignore the uu configuration file.
```
$ echo .uu >> .gitignore
$ git commit -m "Ignore uu configuration file" .gitignore
```

## Upload code via ftp/scp
```
$ uu up
```

## SSH into remote machine
```
$ uu ssh
```

## SSH into remote machine and open DB CLI
```
$ uu dbr
```

## Open DB CLI on local machine
```
$ uu dbl
```



## FAQ

### What does 'uu' stand for?

Unintrusive Uploader



## Contribute

`uu` is developed on Github:  
https://github.com/dotancohen/uu

