
# Level Goal:

The password for the next level is stored somewhere on the server and has all of the following properties:

owned by user bandit7
owned by group bandit6
33 bytes in size

# Solution: 

  * With the following information, we can filter out our required file with the given properties.
  * Also note that the question says that the file lies somewhere on the server, not necessarily in the bandit6 directory. So it is better to find from the root directory itself. Then our search would be across the whole server.
  * So my first plan of action: filter from root!!
  * ![image](https://github.com/user-attachments/assets/0a2248b1-0613-4046-a6e9-1fdc73f9efb0)
  * As you can see, there are many permission denied files. Then I saw that am I getting any file without that error? Because I knew only this that filtering should have worked.
  * And there, amidst the errors, I got what i wanted!!
        ![image](https://github.com/user-attachments/assets/51c9bae8-38f9-4648-95fe-44aee5308384)
  * But if one wants to remove the 'permission denied' errors as well and onnly see the correct output, it is achieved by using '/dev/null' file (a file that desicards anything written to it).
  * This thing can be made to use by piplelining all the output and discarding the ones with error by '2>/dev/null'. Here 2> represents the standard error stream.
