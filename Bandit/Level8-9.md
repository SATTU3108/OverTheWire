
# Level Goal: 

The password for the next level is stored in the file data.txt and is the only line of text that occurs only once

# Solution: 

  * 'uniq' command will fit best according to our needs. Why? We need to filter out the only line that appears once, i.e. is unique in the whole text file. According to man file of 'uniq', -u parameter will help. since it filters the lines that are unique in the text file.
  * According to GfG, The uniq command in Linux is a command-line utility that reports or filters out the repeated lines in a file. In simple words, uniq is the tool that helps to detect the adjacent duplicate lines and also deletes the duplicate lines. uniq filters out the adjacent matching lines from the input file(that is required as an argument) and writes the filtered data to the output file.
  * Since, we need to have the same lines adjacent to each other, we need to sort the lines first in the file.
  * So, command used: "sort data.txt uniq -u"
