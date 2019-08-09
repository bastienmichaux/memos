# Linux commands

## basics

```bash
# what's the current working directory?
$ pwd

# get user name
$ whoami
```

## cd, ls

```bash
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

## display file content

```bash
# first few lines of the file
$ head -n 3 myfile.txt  # first three lines of the file

# last few lines of the file
$ tail -n +4 myfile.txt # the last 4 lines
```

## control execution

```bash
# do something only if the first command succeeds
$ foo && bar # bar is executed only if foo succeeds

# chain commands
$ foo; bar # first execute foo, then execute bar when foo is finished

# execute 2 commands simultaneously
$ foo & bar # bar is executed before foo is finished
```

## users

```bash
# change password for current user
$ passwd
```

## clipboard

in .bashrc: `alias xclip="xclip -selection c"`

```bash
$ echo test | xclip

# or
$ echo arggg | xsel -b
# ctrl+v => arggg
```

[src](https://stackoverflow.com/questions/749544/pipe-to-from-the-clipboard-in-bash-script)

More: [src](https://dev.to/awwsmm/101-bash-commands-and-tips-for-beginners-to-experts-30je)
