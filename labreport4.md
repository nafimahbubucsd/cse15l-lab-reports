# Lab Report 4 

## Doing the steps 4 - 9 from the lab 
---
# Step 4: 

First we log into ssh and clone the new repository we have here

![Image](step1.png)
![Image](step2.png)

I had to loged in with my password as I didnt set up the ssh key yet

# Step 5 
 

`git clone git@github.com:nafimahbubucsd/lab7.git` `<enter>` to clone lab7 repository from my GitHub and it started to clone the repository

![Image](step2.5.PNG)



# Step 6

Running tests:

![Image](step3.png)


`cd lab7` `<enter>` to change directory into lab7 repository to run tests

`javac -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar *.java` `<enter>` to compile all java files in lab7 directory

`java -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar org.junit.runner.JUnitCore ListExamplesTests` `<enter>` to show tests fail





# Step 7

we then edit the file ListExamples file by accessing it in vim, we can do this by typing up `vim ListExamples.java` and we are in vim

![Image](step4.png)

we must first enter INSERT mode in vim by pressing `I`
![Image](step5.png)
Now We can trace where th e Ccrror is at line 44, so I pressed the `<down>` key 44 times

The comment in the code says to change the index1 variable to index2 so i proceeded to do that
![Image](step6.png)
Making sure to exit INSERT mode by pressing `<Escape>`, we can now exit by pressing `:wq` `<enter>` to exit vim and go back to terminal. to exit vim.
![Image](step7.png)
To make sure our changes are saved, we can always check by typing `less ListExamples.java`


# Step 8

Now lets try to run the test again, when we press `<enter>` here are the results 
![Image](step8.png)


The tests do indeed end up passing this time meaning we were able to fix our buggy code in the terminal itself

# Step 9

Our final step just needs us to commit the code to github
![Image](step9.png)
![Image](step10.png)

The first thing we must do is type `git add .<enter>` in order add all the changed files. Then type in `git commit -m "fix"<enter>` to commit the changes, and finally type `git push<enter>` to push the changes. But then it kept asking me for my Username and password, which I did but it did not allow me to push  the changes to the remote repository.
