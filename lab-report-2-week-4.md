# Lap Report 2 - Week 4

## Code Change #1

<img width="770" alt="Screen Shot 2022-04-23 at 5 17 34 PM" src="https://user-images.githubusercontent.com/98578642/164950585-6264deea-a6d2-4070-8350-e6467cd016e8.png"> 

[Test file that prompted me to make change #1](https://github.com/jonathanzhangli/markdown-parser-cse-15l/blob/main/test-file-1.md?plain=1)

<img width="614" alt="Screen Shot 2022-04-23 at 5 37 29 PM" src="https://user-images.githubusercontent.com/98578642/164950768-cb43a72f-2c85-4a11-917d-cabe35b3488d.png">

*the output of running the file at the command line for the version where it was failing*

The initial code had a bug and was causing an index out of range error because it was trying to return a substring at an index that was greater than the inputted string length. To fix this, we changed the while loop to stop another index before the length of the string, which is the index of the last character of the link. 


## Code Change #2

<img width="771" alt="Screen Shot 2022-04-23 at 7 52 00 PM" src="https://user-images.githubusercontent.com/98578642/164954059-3aa43ab4-4cd4-4621-9de5-9e52a4fe321d.png">

[Test file that prompted me to make change #2](https://github.com/jonathanzhangli/markdown-parser-cse-15l/blob/main/test-file-2.md?plain=1)

<img width="619" alt="Screen Shot 2022-04-23 at 8 33 37 PM" src="https://user-images.githubusercontent.com/98578642/164955291-532bd764-cf8b-47f4-a0c6-d5acd2e7ccf7.png">

*the output of running the file at the command line for the version where it was failing*

The test file is empty, as in there are no links. Thus, the pahrentheses and brackets are never found because they are not in the test file. This causes the indexes of the open and close pahrentheses and brackets to be -1, which then causes an index out of bounds error when trying to return the substring at index -1. 


## Code Change #3

<img width="959" alt="Screen Shot 2022-04-24 at 3 11 21 AM" src="https://user-images.githubusercontent.com/98578642/164971529-497a023e-124b-496e-b0d9-56b428c2906d.png">

[Test file that prompted me to make change #3](https://github.com/jonathanzhangli/markdown-parser-cse-15l/blob/main/test-file-3.md?plain=1)

<img width="621" alt="Screen Shot 2022-04-24 at 3 24 42 AM" src="https://user-images.githubusercontent.com/98578642/164971994-e70e11e9-89ce-45e6-8004-eecb5c1d31b8.png">

*the output of running the file at the command line for the version where it was failing*

The initial code had a bug, where it would interpret images as links and print out the image file name as a link in the output. The test file's first "link" is actually an image, which was still printed normally as a link. To fix this bug, we changed the code to detect if the link is an image by checking for "!", and if so then it does not return it. 
