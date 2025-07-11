
# Level Goal: 

The password for the next level is stored in the file data.txt in one of the few human-readable strings, preceded by several ‘=’ characters.

# Solution:

  * As told, the password is preceded by several '=' characters. Now, if password and these equal to signs are on same line, then grep will give our answer.
  * And just fo safety, I will be using "=" only, rather than more than 1. I will get all possible passwords and then depending on what I get, I will figure out what to do next.
  * <img width="549" height="328" alt="image" src="https://github.com/user-attachments/assets/a9271046-0cba-42c2-b32d-ddfca36a1f6b" />
  * Luckily, I get one possible password similar to the format seen till now. And yes, that password works for bandit 10!!
