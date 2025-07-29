
# Level Goal:

The password for the next level is stored in the file data.txt, which is a hexdump of a file that has been repeatedly compressed. For this level it may be useful to create a directory under /tmp in which you can work. Use mkdir with a hard to guess directory name. Or better, use the command “mktemp -d”. Then copy the datafile using cp, and rename it using mv (read the manpages!)

# Solution: 

  * I was actually confused in the question, why it is explicity asking me to create a directory in /tmp. Why can't I make it in the home directory itself. So I tried to create directory with a gibberish name in the home directory. BUt it did not work as such - 'Permission Denied' error comes. Now to sort it out, I thought maybe sudo will work. But it gave this error: "/usr/bin/sudo must be owned by uid 0 and have the setuid bit set"
  * Then I browsed over Stack Overflow to see for the solution. I did come up across a discussion. But according to it. I needed to log out first, then log in as root with the root credentials. But there is no password provided.
  * So the only solution was to go via the steps given, i.e. make a directory within /tmp. The reason that question ask to make a directory with name that is hard to guess is that it will not collide with already exisiting directories present within tmp directory.
  * Now once made the directory, first thing I checked was the file type of the given data.txt file. It is an ASCII text file. So I used 'cat' command to view the contents of the file.
          <img width="636" height="722" alt="Screenshot from 2025-07-29 16-41-20" src="https://github.com/user-attachments/assets/51aba4d7-c19c-4ff0-b183-f50d57d3153e" />
  * Clearly, this is the hexdump of a file. Now we need to reverse the process, ie. rather than creating a hexdump from a file, I need to create a file from the hexdump. For the same 'xxd -r' command is used.
  * Here is the attached screenshot of subsequent steps needed for de-compressing the file back to its originial file!!
            <img width="1358" height="977" alt="Screenshot from 2025-07-29 16-43-47" src="https://github.com/user-attachments/assets/e46134fc-531b-4287-9280-f7489812ad19" />

