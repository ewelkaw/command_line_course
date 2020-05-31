* Redirect data to file
```bash
$ echo "From fairest creatures we desire increase," > sonnet_1.txt
```

* Dump the contents of the file to the screen
```bash
$ cat sonnet_1.txt
```

* Append data to file
```bash
$ echo "From fairest creatures we desire increase," > sonnet_1_lower_case.txt
$ echo "That thereby beauty's rose might never die," >> sonnet_1_lower_case.txt

$ cat line_2.txt line_1.txt > sonnet_1_reversed.txt
```

* Find a difference
```bash
$ diff sonnet_1.txt sonnet_1_lower_case.txt
```

* Listing files and directories
```bash
$ ls
$ ls *.txt
ls -l *.txt   # -l means long form
$ ls -rtl     # list by reversed time of modification (long format)
$ ls -a       # show hidden files (starting with .)
```

* The ls command can be used to check if a file (or directory) exists 
```bash
$ ls foo
ls: foo: No such file or directory
$ touch foo
$ ls foo
foo
```

* Add some type of files to gitignore
```bash
$ echo "*.txt" > .gitignore
$ cat .gitignore
$ ls -a       # you will not see .gitignore without -a option
```

* Command to list all files (including hidden ones) by reverse modification time, in long form
```bash
$ ls -artl
```

* Determine which shell your system is running
```bash
$ echo $SHELL
$ chsh -s /bin/bash   # to change shell
```

* Rename a file
```bash
$ echo "test text" > test
$ mv test test_file.txt
$ ls
test_file.txt
```

* Copy a file 
```bash
$ cp test_file.txt second_test.txt
$ ls
second_test.txt
test_file.txt
```

* Deleting a file
```bash
$ rm second_test.txt
remove second_test.txt? y
$ ls second_test.txt
ls: second_test.txt: No such file or directory
```

Use tab completion for easier work 

* Remove with force (be very careful because it removes all files immediately)
```bash
$ rm -f *.txt
```

* Create an empty file
```bash
touch file_name
```

