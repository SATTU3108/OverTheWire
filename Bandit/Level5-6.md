# Level Goal: 

The password for the next level is stored in a file somewhere under the inhere directory and has all of the following properties:

human-readable
1033 bytes in size
not executable

# Solution: 

  * There are multiple directories present in the directory and out of all, we need to find the file with the desired properties as above. But manually looking for such file would be a very tedious task, since there are multiple files in each directory as well. Some start with hyphen, some are hidden, starting with a dot.
  * In the question, it is given that size of the file is 1033 bytes, so if we can filter out all files that are of this size, our search space will be reduced.
  * So first, I filter the hidden files with size 1033 bytes. (there is only file and that will contain the password).
        ![image](https://github.com/user-attachments/assets/f48bbdab-b5f0-4712-a850-2b6385437385)
