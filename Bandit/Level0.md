# Level Goal: 

The goal of this level is for you to log into the game using SSH. The host to which you need to connect is bandit.labs.overthewire.org, on port 2220. The username is bandit0 and the password is bandit0. Once logged in, go to the Level 1 page to find out.

# Idea:

 * SSH (Secure Shell ) is a parotocol used to securely connect ro remote systems. It is the most common way to access remote Linux servers.
 * If you are using Windows, you’ll need to install a version of OpenSSH in order to be able to ssh from a terminal.
 * Syntax: _ssh://[user@]hostname[:port]_

# Solution:

  * On logging in to the remote server, we can see on using 'ls' command, there is only one file named 'readme' in it.
  * On using 'cat' command on the file by "cat readme", we can see a congratulations message and a password as well.
  * ![Screenshot from 2025-07-07 23-18-42](https://github.com/user-attachments/assets/fa9ea321-1e34-4451-9d4c-95b4a16ea8d9)
