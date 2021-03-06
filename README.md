# Programming-Languages-auto-complete-suggestions
Main Project

In this assignment you will write a C program which produces auto-complete suggestions, similar to what Bash does when beginning to type a command and
pressing . Your program will read all of the file names in a user-provided directory and store them in a data structure made up of an (at least) 26-element 
array of linked lists. You will need to implement a linked list in C. You will have one linked list for each letter of the alphabet, within which you will 
store the filenames which begin with that letter in alphabetical order. After reading the filenames into the array of linked lists, the user will be given 
a “> ” prompt, at which they will enter the beginning of a filename they are interested in. When the user presses enter, all filenames which match that 
prefix will be printed (again, alphabetically). The program will continue to prompt for beginnings of filenames until an empty string is entered.

You may use any built-in C library functions in your program, but you must implement the linked list yourself. You may not use code found on the internet.

Your score will be increased by 10% of the earned score for a successful implementation which uses a prefix tree known as a trie instead of an array of 
linked lists. Your implementation must be your own.

Sample Interaction

$ ./filecomplete
 
Enter a folder name: /usr/bin
&gt; zi

Files starting with zi in /usr/bin:
zip 
zipcloak 
zipgrep 
zipinfo 
zipnote 
zipsplit 

&gt; zipc
Files starting with zipc in /usr/bin:

zipcloak
