# Week 2 Lab Report
*Read for a tutorial on how to log into a course-specific account on ieng6!*

## Installing VScode
Go to the [VS Code website](https://code.visualstudio.com/).

<img width="716" alt="Screen Shot 2022-04-09 at 11 33 54 PM" src="https://user-images.githubusercontent.com/98578642/162605606-aaadbbdb-aa46-4f20-9b3e-f78215567e26.png">

Click on the blue download button and follow the given installation steps! Then you're good to go :-)

## Remotely Connecting
Open a terminal in VS Code and then use the ssh command followed by your username.

Example:

`$ ssh cs15lsp22zz@ieng6.ucsd.edu`

Say yes to connect to the server for the first time!

**Almost there!** Now just type in your password, and you're in!

It should look something like this when you're logged in:

<img width="510" alt="Screen Shot 2022-04-09 at 11 56 41 PM" src="https://user-images.githubusercontent.com/98578642/162606364-99c3e22f-9f11-48af-a71f-6c4e7caff126.png">

## Trying Some Commands
Play around and run some commands such as cd, ls, pwd, mkdir, & cp!

These are a few you can try:

`cd

ls -lat

cp /home/linux/ieng6/cs15lsp22/public/hello.txt ~/

cat /home/linux/ieng6/cs15lsp22/public/hello.txt`

This is the result of some of these commands!

<img width="446" alt="Screen Shot 2022-04-10 at 12 02 15 AM" src="https://user-images.githubusercontent.com/98578642/162606494-d8d51d4e-aa3d-49e6-8d59-b147351cff2d.png">

*very cool*

## Moving Files with scp

First step is getting a file :D and then run javac and java on it!

After that, run this command:

`scp file.java cs15lsp22zz@ieng6.ucsd.edu:~/`

*(replacing file.java with your file and cs15lsp22zz@ieng6.ucsd.edu with your own username)*

Put in your password and then you're good to go ! 

It should look like this:

<img width="459" alt="Screen Shot 2022-04-10 at 12 09 10 AM" src="https://user-images.githubusercontent.com/98578642/162606726-ced4e097-cb78-42e6-9e24-61d3bd20ac38.png">

## Setting an SSH Key

First off, let's create the private key (id_rsa) and public key (id_rsa.pub) and store it in the .ssh directory on your device.

Enter this command:
`$ ssh-keygen`

Then enter this:

Enter file in which to save the key 

(/Users/<user-name>/.ssh/id_rsa): /Users/<user-name>/.ssh/id_rsa
  
After that, **DON'T** add a passphrase!
  
To copy the public key to the ssh directory on the server, go on server and use these commands:
 
$ ssh cs15lsp22zz@ieng6.ucsd.edu
$ mkdir .ssh

Then log out :)

On the client, use this command:
$ scp /Users/<user-name>/.ssh/id_rsa.pub cs15lsp22zz@ieng6.ucsd.edu:~/.ssh/authorized_keys
  
Then you can log in with no password each time!!! *YAY* See look-
  
  <img width="456" alt="Screen Shot 2022-04-10 at 12 17 09 AM" src="https://user-images.githubusercontent.com/98578642/162607068-eb2abacb-23c6-4f83-ba12-32834271ca5a.png">

No password! **amazing**
  
## Optimizing Remote Running
  
  Here are some tips to optimize!
  * write a command in quotes after an ssh command to run it on the remote server
  * semicolons run multiple commands on the same line

<img width="461" alt="Screen Shot 2022-04-10 at 12 19 30 AM" src="https://user-images.githubusercontent.com/98578642/162607177-afafbb3f-f624-4c24-85e0-9a09e2419376.png">

  I copied a file to the remote server and ran it in one line!! ^
  
**Hope that helped :-)**
  

