# Copying whole directories with ```scp -r```
It will be very convienient to copy over entire folders onto remote servers,
rather than ```scp``` individual files one by one - thats too time consuming.

To do so, we will let ```scp``` copy recursively, with:

```$ scp -r . cs15lwi22akj@ieng6.ucsd.edu:~/markdown-parse``` 
cs15lwi22akj is my account name. It should vary depending on your remote server access
 
```-r``` tells ```scp``` to work recursively.\
```.``` means the source, the currenty directory. \
```~/markdown-parse``` tells ```scp``` to create ```markdown-parse``` directory on the remote server and then copy the current directory to there.

 Doing so, you copy all files onto the directory.\
 ![Image](sc1.png)
This copied ALL files onto the a new markdown-parse folder, and we can run these programs.\
![Image](sc2.png)
An alternate way to copy files is\
```scp -r *.java *.md /lib``` copies only files that end with ```.java```, ```.md``` and ```/lib```\

Now, we can run it all in one line.
Copying all the files we want and runnning the JUnit test.

![Image](sc3.png)
![Image](sc4.png)