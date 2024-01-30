## Level 11 (Choose your path2)

 - First, create a symbolic link named "wc" in your home directory pointing to the executable file /bin/sh
 

    ` ln -s /bin/sh ~/wc`

 - Then, execute charp2 while temporarily modifying the PATH to search for executables only in the current directory. After that, use "cat" to display the content of the solution.txt file, redirecting the output to the standard error stream.
 
    `PATH=~ ./charp2 "/bin/cat solution.txt 1>&2"`
