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

