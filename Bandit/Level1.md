
# Level Goal:

The password for the next level is stored in a file called readme located in the home directory. Use this password to log into bandit1 using SSH. Whenever you find a password for a level, use SSH (on port 2220) to log into that level and continue the game.

# Solution: 

  * First exit as the current user 'bandit0' by using exit command and then connect to the bandit1, using password obtained in level 0.
  * On logging in, we see that only a dashed character file is being shown. Cat command fails to open this file.
  * On looking up the Internet, I saw the reason behind id that on typing in 'cat -', the hyphen seems to feel like an argument, after which another character will come and then cat command will be interpreted.
  * But I want to view the contents of this file? How do I do that? -> The solution is to add prefix the path of the file to the cat command.
  * ![Screenshot from 2025-07-07 23-33-27](https://github.com/user-attachments/assets/d9f2d8d0-a12b-431c-b5eb-2770520bff73)
  * In the image above, you can see that I had to interrupt the simple cat command. The reason behind id that it was waiting for input argument on screen.
