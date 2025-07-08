# Level Goal: 

The password for the next level is stored in the only human-readable file in the inhere directory. Tip: if your terminal is messed up, try the “reset” command.

# Solution:

  * There are a bunch of files in the only directory present for the user 'bandit4'
            ![Screenshot from 2025-07-08 10-09-11](https://github.com/user-attachments/assets/6abd2db7-fa03-40f6-840b-6c4824e352eb)
  * In the question, it is given there is only 1 human readable file. The main objective here would be to determine that file. One way to do this is to actually use cat command on the 9 files given. And the only file that would not containg gibberish os the file that contains the password.
  * Above method works here since there are only 9 files. However, if there would be multiple files, then we would be in trouble manually seeing contents of all the files!!
  * One way to solve this is by actually determing the file type of each file, our required file would contain ASCII text, one that is interepretable.
  * In order to determine the filetype of any file, 'file' command is used. Now in order to use this command for all the files present in the directory, first notice that all files are starting with a hyphen, just like in level1-2. Then use the following commmand "file ./-*"
  * What this command does that in the current directory, it gives file type of all files starting with a hyphen.
        ![image](https://github.com/user-attachments/assets/7e428809-815e-4a04-9e82-75600c475b55)
  * See that -file07 contains ASCII text and on using cat command there, we can clearly see that yes, we get the password!!

