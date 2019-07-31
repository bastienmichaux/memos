# Linux commands

basics

```shell
# what's the current working directory?
$ pwd

# get user name
$ whoami
```

cd, ls

```shell
# change working directory
$ cd path/to
$ cd .. # go to parent directory
$ cd -  # go to previous location
$ cd ~  # go to user's home
$ cd /  # go to top-most directory


# list files
$ ls
$ ls -a # show hidden files
$ ls -l # more details
```

display file content

```shell
# first few lines of the file
$ head -n 3 myfile.txt  # first three lines of the file

# last few lines of the file
$ tail -n +4 myfile.txt # the last 4 lines
```

control execution

```shell
# do something only if the first command succeeds
$ foo && bar # bar is executed only if foo succeeds

# chain commands
$ foo; bar # first execute foo, then execute bar when foo is finished

# execute 2 commands simultaneously
$ foo & bar # bar is executed before foo is finished
```
