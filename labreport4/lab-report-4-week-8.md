# Week 8 Lab Report
For each snippet, here are the expected outputs:

Snippet 1: ```[]``` \
Snippet 2: ```[]``` \
Snippet 3: ```[]``` 

Since all of the test cases give the links with incorrect formatting,
the results should not produce incorrect link formatting, thus all of
them should be empty.

Their group's code:
The JUnit test I used ![Image](thetest.png)
The output I got: ![Image](runtest.png)
Our group's (my) code:
The JUnit test I used ![Image](mytests.png)
The output I got: ![Image](myresult.png)

The other group's implementation passed, but mine failed.

## Questions
Do you think there is a small (<10 lines) code change that will make your program work for snippet 1 and all related cases that use inline code with backticks? If yes, describe the code change. If not, describe why it would be a more involved change.

A check for backticks could be added to my implementation of MarkdownParse. Similar to how I checked for other unwanted symbols in the link and the brackets before and if there is an exclamation point. If backticks are fine within the code, (I dont know the specifications of embedding links), then you can do a String replace ` with empty space. 

Do you think there is a small (<10 lines) code change that will make your program work for snippet 2 and all related cases that nest parentheses, brackets, and escaped brackets? If yes, describe the code change. If not, describe why it would be a more involved change.

For unwanted symbols, you can do an if statement that checks if any of the parentheses, brackets, etc are in the link. If so, do not print out the link.

Do you think there is a small (<10 lines) code change that will make your program work for snippet 3 and all related cases that have newlines in brackets and parentheses? If yes, describe the code change. If not, describe why it would be a more involved change.

I think to check for newlines, you can have an if statment to see if there is a newline during the creation of the code. A newline may appear before the parentheses or after and by checking that location for newlines, you can decide whether or not to print the code.


