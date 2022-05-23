# Week 8 Lab Report 4

## What Each Snippet *Should* Produce

*I decided the expected outputs using CommonMark and choosing the links that were turned into blue hyperlinks.*

**Snippet 1:**

<img width="697" alt="Screen Shot 2022-05-22 at 9 35 29 PM" src="https://user-images.githubusercontent.com/98578642/169744076-b6731468-4b15-425c-9ed8-02ec7ce6adbb.png">

--

Expected Output: 

\`google.com



**Snippet 2:**

<img width="698" alt="Screen Shot 2022-05-22 at 9 37 37 PM" src="https://user-images.githubusercontent.com/98578642/169744341-e4f89cef-ac54-4b61-ac7a-86dc5393f5d5.png">

--

Expected Output: 

a.com

a.com(())

example.com



**Snippet 3:**

<img width="690" alt="Screen Shot 2022-05-22 at 9 40 43 PM" src="https://user-images.githubusercontent.com/98578642/169744667-4129a46b-6ce5-4094-8a9d-b57c5a2a29d8.png">

--

Expected Output:
https://sites.google.com/eng.ucsd.edu/cse-15l-spring-2022/schedule 

## My Implementation

Code for the Tests:

<img width="788" alt="Screen Shot 2022-05-22 at 10 31 18 PM" src="https://user-images.githubusercontent.com/98578642/169749863-73597e4a-161e-4fe5-bccb-ebb744d5271a.png">

Test Output:

<img width="646" alt="Screen Shot 2022-05-22 at 10 22 20 PM" src="https://user-images.githubusercontent.com/98578642/169748900-0527c5b4-b8aa-413d-9852-ddb0ced4615b.png">

All 3 snippet tests failed. Snippet 1 & 2 failed due to an Assertion Error, whereas Snippet 3 failed due to a StringIndexOutOfBoundsException Error. 

## Implementation I reviewed

Code for the Tests:

<img width="809" alt="Screen Shot 2022-05-22 at 10 29 54 PM" src="https://user-images.githubusercontent.com/98578642/169749715-6b96086f-6f49-44e3-8aed-8e79743bb270.png">

Test Output:

<img width="521" alt="Screen Shot 2022-05-22 at 9 48 35 PM" src="https://user-images.githubusercontent.com/98578642/169745453-9f12eb1a-53eb-40ff-8dcf-96bdae555186.png">

All 3 snippet tests failed. Snippet 1 & 2 failed due to an Assertion Error, whereas Snippet 3 failed due to a StringIndexOutOfBoundsException Error. 

## Potential Code Changes

1. To get the other links to work, I could make the code start reading from the last closing bracket. To do this, I could use if else statements to see if there is a backtick before the last closing bracket and if there are more than one closing brackets. 
2. To fix this program, I could use a while statement and the indexOf() method to find the last closing bracket. I would also check that the brackets are in pairs. Then this would start reading the link from the last closing bracket. 
3. To account for all cases that have new lines in brackets and parentheses, I would use indexOf to check that the ending closing pahrentheses and brackets exists and go to the next line if the current line ends. This would allow all brackets and pahrentheses to be accounted for even if there are line breaks. 

