`sudo` gives ordinary users the power to execute commands as the superuser

* Making directories
```bash
$ mkdir text_files
$ mv *.txt text_files/    # move the text files there using a wildcard
$ ls text_files/
```

* Show just the directory using the -d option
```bash
$ ls -d text_files/
$ ls -ld text_files/    # longer info 
```

* change directories using cd 
```bash
$ cd text_files/
$ cd                    # go to home dir
$ cd ~                  # go to home dir
```

* print working directory command 
```bash
$ pwd
```

* Make new directory
```bash
$ mkdir second_directory
```

* Working in current directory
```bash
$ find . -name '*.txt'    # find in workdir by name files ending with .txt
$ open .                  # open current directory
```

* Renaming directory
```bash
$ mv foo/ bar/
$ mv bar foo
```

* Copying directory
```bash
$ cp -r ../text_files .   # -r means recursive, so down the tree and dot means to current dir
```

* Deleting directory
```bash
$ rmdir second_directory  # we can't do this if dir is not empty, we need to do it recursively
$ rm -rf second_directory/
$ ls second_directory
```

* Grep redux
```bash
$ cd text_files/
$ mkdir foo
$ cd foo/
$ echo sesquipedalian > long_word.txt
$ cd
$ grep sesquipedalian text_files      # this doesn't work.
$ grep -ir sesquipedalian text_files  # that will work grep recursively (case-insensitive)recursively 
```