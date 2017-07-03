# ls

-l long format, displaying Unix file types, permissions, number of hard links, owner, group, size, last-modified date and filename

-f do not sort. Useful for directories containing large numbers of files.

-F appends a character revealing the nature of a file, for example, * for an executable, or / for a directory. Regular files have no suffix.

-a lists all files in the given directory, including those whose names start with "." (which are hidden files in Unix). By default, these files are excluded from the list.

-R recursively lists subdirectories. The command ls -R / would therefore list all files.

-d shows information about a symbolic link or directory, rather than about the link's target or listing the contents of a directory.

-t sort the list of files by modification time.

-h print sizes in human readable format. (e.g., 1K, 234M, 2G, etc.) 

# cat
cat [options] [file_names]

The output of cat may be redirected to a file:

cat [options] [file_names] > newfile.txt

or it may be redirected as input to another program, e.g.:

cat file1 file2 | less

which invokes the less paging utility.


    -b (GNU: --number-nonblank), number non-blank output lines
    
    -e implies -v but also display end-of-line characters as $ (GNU only: -E the same, but without implying -v)
    
    -n (GNU: --number), number all output lines
    
    -s (GNU: --squeeze-blank), squeeze multiple adjacent blank lines
    
    -t implies -v, but also display tabs as ^I (GNU: -T the same, but without implying -v)
    
    -u use unbuffered I/O for stdout. POSIX does not specify the behavior without this option.
    
    -v (GNU: --show-nonprinting), displays nonprinting characters, except for tabs and the end of line character

cat file1.txt 	                                  -Display contents of file

cat file1.txt file2.txt 	                      -Concatenates 2 text files and will show them in the terminal

cat file1.txt file2.txt > newcombinedfile.txt     -Concatenates 2 text files and writes them to a new file

cat >newfile.txt 	                              -Creates a file called newfile.txt - type the desired input and press CTRL+D to finish. The text will be in file newfile.txt.

cat -n file1.txt file2.txt > newnumberedfile.txt  -Some implementations of cat, with option -n, can also number lines

cat file1.txt > file2.txt 	                      -Redirects standard output of a file into a new file

cat file1.txt >> file2.txt 	                      -Appends standard output of a file into a new file

cat file1.txt file2.txt file3.txt | sort > test4  -Output of cat command is piped to sort and result will be redirected in a newly created file.


** dashed file open = cat ./-
** spaced file open = cat file\ name\ .txt

# du

    -a, In addition to the default output, include information for each non-directory entry
    -c, display a grand total of the disk usage found by the other arguments
    -d #, the depth at which summing should occur. -d 0 sums at the current level, -d 1 sums at the subdirectory, -d 2 at sub-subdirectories, etc.
    -H, calculate disk usage for link references specified on the command line
    -k, show sizes as multiples of 1024 bytes, not 512-byte
    -L, calculate disk usage for link references anywhere
    -s, report only the sum of the usage in the current directory, not for each file
    -x, only traverse files and directories on the device on which the pathname argument is specified. 
