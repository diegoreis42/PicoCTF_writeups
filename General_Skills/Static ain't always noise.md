# Static ain't always noise

## Description 
Can you look at the data in this binary: static? This BASH script might help!

## Solution

 It's pretty easy, one of the most basics ways to analyze if have something hidden in a file is using the command [strings](https://www.man7.org/linux/man-pages/man1/strings.1.html), it can ~as i expected you read~ print
 sequences of printable characteres in a file. And with [grep](https://manpages.org/grep/1), we can search for our flag, like this:
 
 > strings -a static | grep pico
 
 This " | " (pipeline) operator, take the output of the previous command and give as a input to the second command. 
 
