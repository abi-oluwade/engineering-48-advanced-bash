# Advanced Bash

We will cover concepts as well as commands in bash.
--help will give us documentation, e.g 'grep --help'

## commands

ctrl+c can get us out of issues.
chmod [permission] <path or file>
e.g: chmod 0700 <path-to-file>
- head
  - cat and head -(x) can give us the text details of a file in Bash
  - tail
  - sort
  - nl numbers the line of the text
  - wc (word count, gives number of new-lines, words, byte count)
 "* and __ can be used as wildcards"

- STDIN-->0, STDOUT-->1, STDERR-->2
these all have numbers, that identify them.

- Piping and redirection
piping is when you basically join two programs together so that they run.
ls >directory.txt for example redirects the out put to that command.
so now 'cat directory.txt' will act like ls
(> = redirects STDOUT to what you assign it to)

(|) lets you pipe together commands.
````
$ls missing_directory
> ls: cannot access 'missing_directory': No such file or directory
$ls missing_directory>2 ls_log.text
$ cat ls_log.txt
> ls: cannot access 'missing_directory': No such file or directory

````
Two >> will append the error message
grep = get regular expressions. we can use it to search, it can search files and inside files.
eg 'cat example.txt | grep text' will search the example.txt file and look for the
word text throughout it.
grep -v will filter out files that DO have the text string in them.

## concepts


- extension-less
- everything is a file.
- bash is case sensitive -- (especially searching)
- STDIN(input fed into program), STDOUT(what comes out of that prog),
  STDERR(provides the error message)
