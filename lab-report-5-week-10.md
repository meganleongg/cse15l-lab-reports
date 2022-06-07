# Week 10 Lab Report

## Using vimdiff to Find Tests with Different Results

<img width="975" alt="Screen Shot 2022-06-06 at 10 51 27 PM" src="https://user-images.githubusercontent.com/98578642/172306100-35f33889-fb6f-41c1-8b52-956fec75b8e5.png">

I used vimdiff to compare the test outputs for the two repositories. From this, I chose to use test files 201 and 489. 

[Link to test file 201](https://github.com/nidhidhamnani/markdown-parser/blob/main/test-files/201.md)

[Link to test file 489](https://github.com/nidhidhamnani/markdown-parser/blob/main/test-files/489.md)

## Expected Output for Test 201 versus Actual Outputs

<img width="1046" alt="Screen Shot 2022-06-06 at 11 26 51 PM" src="https://user-images.githubusercontent.com/98578642/172310673-dbda37fe-48a4-4133-ba5e-e6634643618e.png">

The expected output is []. 

Provided Repo Output (Incorrect):

[baz]


My Repo (Correct):
[]

<img width="957" alt="Screen Shot 2022-06-06 at 11 33 20 PM" src="https://user-images.githubusercontent.com/98578642/172311723-bbfe9f0e-2c7c-46b4-962e-1b22f5db4193.png">

## Expected Output for Test 489 versus Actual Outputs

<img width="967" alt="Screen Shot 2022-06-06 at 11 34 33 PM" src="https://user-images.githubusercontent.com/98578642/172311952-203ded1a-35c0-4b82-9fbd-424c8f39ffed.png">

The expected output is []. 


Provided Repo Output (Incorrect):

[foo

bar]


My Repo (Correct):
[]

<img width="968" alt="Screen Shot 2022-06-06 at 11 37 32 PM" src="https://user-images.githubusercontent.com/98578642/172312429-3473c27f-6544-4daa-9bc6-bbc71214084c.png">
