* Downloading a file
```bash
$ which curl
$ curl -OL https://cdn.learnenough.com/sonnets.txt
$ ls -rtl
$ !curl     # to run the last curl command
```

* Looking at the head of the sample text file
```bash
$ head sonnets.txt
```

* Looking at the tail of the sample text file 
```bash
$ tail sonnets.txt
```

* wordcount file
```bash
$ wc sonnets.txt
```

* Redirecting head and running wc on the result
```bash
$ head sonnets.txt > sonnets_head.txt 
$ wc sonnets_head.txt 
```

* Piping the result of head through wc 
```bash
$ head sonnets.txt | wc
```

* Grepping
```bash
$ grep rose sonnets.txt           # finding the occurrences of “rose” in Shakespeare’s sonnets
$ grep rose sonnets.txt | wc      # piping the results of grep to wc
$ grep -i rose sonnets.txt | wc   # doing a case-insensitive grep
$ grep ' ro[a-z]*s ' sonnets.txt  # grep of all words starting from ro and ending by s

# grep program by name and kill it
$ ps aux | grep spring
$ kill -15 12241
```

* Show processes (sorted)
```bash
$ top
```

* Ping a server URL
```bash
$ ping google.com
```