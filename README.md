# fup

CLI script for uploading code and performing other common operations on a remote server



## Description

`fup` is used to easily upload code, access SSH, and access a remote database on remote servers. It supports both FTP and SCP methods of code upload, and of course supports the use of public/private keys for connecting via SSH. It searches each successive parent directory for a `.fup` configuration file, allowing one to use it in any project directory. The `.fup` confige file should not be added to Git or other version control system as it is likely to contain sensitive information.



# Using fup

## Confige fup
```
$ vim .fup
```

## Instruct Git to ignore the fup configuration file.
```
$ echo .fup >> .gitignore
$ git commit -m "Ignore the fup configuration file" .gitignore
```

## Upload code via ftp/scp
```
$ fup up
```

## SSH into remote machine
```
$ fup ssh
```

## SSH into remote machine and open DB CLI
```
$ fup dbr
```

## Open DB CLI on local machine
```
$ fup dbl
```



## FAQ

### What does 'fup' stand for?

FTP Uploader



## Contribute

`fup` is developed on Github:  
https://github.com/dotancohen/fup

