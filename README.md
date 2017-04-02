# ffu

CLI script for uploading code and performing other common operations on a remote server



## Description

`ffu` is used to easily upload code, access SSH, and access a remote database on remote servers. It supports both FTP and SCP methods of code upload, and of course supports the use of public/private keys for connecting via SSH. It searches each successive parent directory for a `.ffu` configuration file, allowing one to use it in any project directory. The `.ffu` confige file should not be added to Git or other version control system as it is likely to contain sensitive information.



# Using ffu

## Confige ffu
```
$ vim .ffu
```

## Instruct Git to ignore the ffu configuration file.
```
$ echo .ffu >> .gitignore
$ git commit -m "Ignore ffu configuration file" .gitignore
```

## Upload code via ftp/scp
```
$ ffu up
```

## SSH into remote machine
```
$ ffu ssh
```

## SSH into remote machine and open DB CLI
```
$ ffu dbr
```

## Open DB CLI on local machine
```
$ ffu dbl
```



## FAQ

### What does 'ffu' stand for?

Fast File Uploader



## Contribute

`ffu` is developed on Github:  
https://github.com/dotancohen/ffu

