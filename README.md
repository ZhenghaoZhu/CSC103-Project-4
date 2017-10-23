# CSC103-Project-4

**Uniq**
For this, the only options you need to make work are -c (show the count before each line), -d (only show duplicated lines), and -u (only print unique lines).
wc (word count)
You should implement the standard -c,-l,-w,-L options, as well as a new -u option which is explained below. Without arguments, it should print the line, word, and byte counts, just as the system’s wc. A few differences from the system’s version:
1. You don’t need to process arguments (like filenames); you can assume that all the input comes from standard input.
2. You don’t need to format the output exactly the same way as wc: you can just separate each piece of the output by a tab \t character, or a few spaces (but don’t print anything that isn’t whitespace between the output fields).
3. You should add a --uwords option which counts the unique words.

Sample Output from the program:
> $ echo "this is a test" | ./wc
        1       4        15
      
The format of the output is:

#lines #words #bytes [longest line len] #uniquewords

with each separated by whitespace (you can use tabs if you want). If no options are given, just print the first 3 items above, just like normal wc would do. Otherwise, print only the values corresponding to the flags your program was given, and output them in the same order as above.

**shuf**

This just permutes the lines of the input. It is important that each permutation is equally likely to be selected. You should implement the options -e,-i,-n.

**sort**

You just need to sort the lines of the file. The only options you need to worry about are -r (sort descending), -u (don’t print duplicates) and -f (ignore the case).

**tr**

This translates characters from one set to another set. The only options you need to worry about are -c,-d. To make things easier, you don’t need to worry about the character classes at all, although you should make your program work with at least the escape sequences \\,\n,\t.
