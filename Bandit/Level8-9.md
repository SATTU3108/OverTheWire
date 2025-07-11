
# Level Goal: 

The password for the next level is stored in the file data.txt and is the only line of text that occurs only once

# Solution: 

  * 'uniq' command will fit best according to our needs. Why? The solution that I have come up with is to count the occurences of each line and the line with the occurence of 1 is our desired answer.
  * According to GfG, The uniq command in Linux is a command-line utility that reports or filters out the repeated lines in a file. In simple words, uniq is the tool that helps to detect the adjacent duplicate lines and also deletes the duplicate lines. uniq filters out the adjacent matching lines from the input file(that is required as an argument) and writes the filtered data to the output file.
  * Since, we need to have the same lines adjacent to each other, we need to sort the lines in the file.
  * So, command used: "sort data.txt uniq -c"
