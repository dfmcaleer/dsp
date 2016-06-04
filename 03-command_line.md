# Learn command line

Please follow and complete the free online [Command Line Crash Course
tutorial](http://cli.learncodethehardway.org/book/). This is a great,
quick tutorial. Each "chapter" focuses on a command. Type the commands
you see in the _Do This_ section, and read the _You Learned This_
section. Move on to the next chapter. You should be able to go through
these in a couple of hours.

---

###Q1.  Cheat Sheet of Commands  

Make a cheat sheet for yourself: a list of at least **ten** commands and what they do, focused on things that are new, interesting, or otherwise worth remembering.

*  Used when you want to find all of something, for example, ls *.txt finds all text files.

|  Get the output from the left command and give it to the command on the right.

<  Get input from file on the right and use it for command on the left.

>  Takes output from left command and writes it to a file.

cat  Prints a whole file, or use to type things directly into a file: cat > filename.txt  (Use ctrl-d to exit.)

cd .. goes up one directory, cd ../.. goes up two, etc.  Can move around directory tree this way as well.

cp originalfilename newfilename  Copies file or directory.  Can also copy it somewhere else with: cp filename newdirectory/

grep  Finds things inside files.  grep searchterm filename

mv  move a file or directory ann rename

man  To get help (read manual)

rm filename  Removes files
rmdir directoryname  Removes directories




---

###Q2.  List Files in Unix   

What do the following commands do:  
`ls`  
`ls -a`  
`ls -l`  
`ls -lh`  
`ls -lah`  
`ls -t`  
`ls -Glp`  

ls  Lists contents of the directory where you are.

ls -a  Lists all files including hidden files.

ls -l  List with long format (shows permissions, when created, etc.)

ls -lh  List with long format and readable file size.

ls -lah  List with long format and readable file size for all files including hidden ones.

ls -t  Sort list by time and date.

ls -Glp  The -G option enables colorized output (links will be blue), -l is long format, and -p adds / at the end of the directory name.
---

###Q3.  More List Files in Unix  

Explore these other [ls options](http://www.techonthenet.com/unix/basic/ls.php) and pick 5 of your favorites:

ls -d  Displays only directories.

ls -m  Displays names as comma-separated list.

ls -q  Displays non-printing characters as ?.

ls -R  Displays sub-directories as well.

ls -r Displays in reverse order.

---

###Q4.  Xargs   

What does `xargs` do? Give an example of how to use it.

xargs reads space, tab, newline, and end-of-file delimited strings from standard input and executes with strings as arguments.  Can be used to remove or do an operation on a list of filenames.

Example:  find ./temp -print | xargs grep "June"

Find all files in the temp folder, pass to grep, and search for June.

 

