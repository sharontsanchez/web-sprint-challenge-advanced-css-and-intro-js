# Sprint Challenge: Advanced CSS and Intro to JavaScript - Influential Artists

**Read these instructions carefully. Understand exactly what is expected _before_ starting this Sprint Challenge.**

This challenge allows you to practice the concepts and techniques learned over the past week and apply them in a concrete project. This Sprint explored advanced CSS and introductory JavaScript concepts. During this Sprint, you studied responsive web design, variable declaration, conditionals, loops, functions, arrays, and objects. In your challenge this week, you will demonstrate proficiency by creating a website of influential artists with data from an object.

This is an individual assessment. All work must be your own. Your challenge score is a measure of your ability to work independently using the material covered through this sprint. You need to demonstrate proficiency in the concepts and objectives introduced and practiced in preceding days.

You are not allowed to collaborate during the Sprint Challenge. Your work reflects your proficiency in Responsive Design, and JavaScript Basics.


## Introduction

In this challenge, you will use a data set of artists to build an "influential artists" webpage. This data comes from a set of "50 influential artists" on [Kaggle](https://www.kaggle.com/ikarus777/best-artworks-of-all-time). We have reduced the data to just 20 artists to make it slightly easier to work with.

### Commits

Commit your code regularly and meaningfully. 

## Interview Questions
### (please edit this file and write your answer below each question.)

Please answer the following questions below, you may edit the readme file to include your answers below the question.


1. How would you describe acessibility on the web to someone new to programming?

When someone describes a site as "accessible," they mean that any user can use all its features and content, regardless of how the user accesses the web — even and especially users with physical or mental impairments.

Accessibility is the practice of making your websites usable by as many people as possible. We traditionally think of this as being about people with disabilities, but the practice of making sites accessible also benefits other groups such as those using mobile devices, or those with slow network connections. 

Accessible sites present information through multiple sensory channels, such as sound and sight, and they allow for additional means of site navigation and interactivity beyond the typical point-and-click-interface: keyboard-based control and voice-based navigation. The combination of a multisensory approach and a multi-interactivity approach allows disabled users to access the same information as nondisabled users.

Building accessible sites benefit everyone:

Semantic HTML, which improves accessibility, also improves SEO, making your site more findable.
Caring about accessibility demonstrates good ethics and morals, which improves your public image.
Other good practices that improve accessibility also make your site more usable by other groups, such as mobile phone users or those on low network speed. In fact, everyone can benefit from many such improvements.

2. Talk about 3 different things you can do to ensure your website is accessible. 

a. Include proper alt text for images.
Images should include Alt text in the markup/code; complex images should have more extensive descriptions near the image (perhaps as a caption or descriptive summaries built right into a neighboring paragraph)

b. Use color with care.
use color, but also be sure to use other visual indicators, such as an asterisk or question mark. Be sure to also distinguish blocks of content from one another using visual separation (such as whitespace or borders). This will consider both people with color deficiency as well as other groups of people with disabilities particularly users with learning disabilities, benefit greatly from color when used to distinguish and organize your content.

c. Use Semantic HTML tags to structure your page
use of semantic HTML provides accessibility, SEO (search engine optimization) and helps other developers to read your work at ease. When it is used correctly and stragetically,  the content of your website will be well-organized and easily interpreted by screen readers and others with disabilities. 


3. How would you explain the concept of a variable to someone new to programming?

Variables are containers for store, change and use data in code. They also provide a way of labeling data with a descriptive name, so our programs can be understood more clearly by the reader and ourselves. It is helpful to think of variables as containers that hold information. Their sole purpose is to label and store data in memory. This data can then be used throughout your program.
The syntax to create a variable is first the keyword, a space, the name we are giving the variable, an equal sign, the value we are assigning the variable, and then a semicolon. 

There are 3 ways to declare a JavaScript variable: var, let and const.
There are differences between them

Var
- can be reassigned
- can also be redeclared
- function scoped

Let
- can be reassigned
- cannot be redeclared 
- block scoped 


Const
- cannot be reassigned
- cannot be redeclared
- block scoped 

All JavaScript variables must be identified with unique names.

These unique names are called identifiers. Identifiers can be short names (like x and y) or more descriptive names (age, sum, totalVolume).

The general rules for constructing names for variables (unique identifiers) are:
Names can contain letters, digits, underscores, and dollar signs.
Names must begin with a letter
Names can also begin with $ and _ (but we will not use it in this tutorial)
Names are case sensitive (y and Y are different variables)
Reserved words (like JavaScript keywords) cannot be used as names

4. What is the purpose of using functions in code?

A function is simply a “chunk” of code that you can use over and over again, rather than writing it out multiple times. Functions enable programmers to break down or decompose a problem into smaller chunks, each of which performs a particular task.
The first reason is reusability. Once a function is defined, it can be used over and over and over again. You can invoke the same function many times in your program, which saves you work.
The second reason is abstraction. In order to use a particular function you need to know the following things:
The name of the function;
What the function does;
What arguments you must give to the function; and
What kind of result the function returns.

5. How do you access a key inside of an object inside of an array?

We can access an item at any time in an array, we just need to call the item by its position in the array. Items are given a numerical position (index) according to where it is in the array, in order. An array's numerical order ALWAYS starts at 0, so the first item is in the 0 index, the second in the 1 index, the third in the 2, and so on.
But when we store a key inside of an object inside of an array, we have to invoke a function to call out the specific key at the specific index in that array into a new array = []; looping through the array and pushing out the key we require or want in the array. We can do that by setting a new array name to equal to [] and using the for loop statement " for (i = 0; i <= array.length-1; i++){}. 

function findAString(array, string, key, key2){
  const results = []; // creating an empty array so that we can push our results to it 
  for(let i = 0; i < array.length; i++){ // writing a for loop so we can search through the entire array provided 
    if(array[i][key].includes(string)){ // condition - if the array provided and the key provided includes the string provided then
      results.push(array[i][key2]); // push that array and other key to the empty results array 
    } 
  }
  return results; // outside of the loop because we want to return the results after we've looped through the entire array
}

You are expected to be able to answer questions in these areas. Your responses contribute to your Sprint Challenge grade. 

## Instructions

### Task 1: Project Set-Up

Follow these steps to set up your project:

1. Fork the repo
2. Clone your forked version of the repo
3. cd into your repo and create a branch with your first and last name
NOTE: Tests will run for the JavaScript portion of this challenge only
4. open the terminal in your vs code and type `npm install`
5. next type `npm run test` in your terminal
6. Complete your work making regular commits, once you have all your tests passing and you are ready to submit your work please see canvas for instructions on how to submit

### Testing & Debugging

Open a second terminal inside of your project by clicking on the split terminal icon
![alt text](assets/split_terminal.png "Split Terminal")

Inside of your second terminal type `npm start` 
![alt text](assets/npm_start.png "type npm start")

You will be running your tests in one terminal and debugging in the other. As you work on your code you should make use of `console.log` to check your progress and debug.
![alt text](assets/tests_debug_terminal_final.png "your terminal should look like this")

### Task 2a:  Minimum Viable Product - Responsive Design

*Before you jump in, take 10 minutes to review the code that has already been provided for you. Take time to see how the home page was built. During this time, [Review the provided design files](design/). You have been provided all content necessary in the [index.html file](index.html) and basic styling in the [index.css file](css/index.css).*

* [ ] Ensure your website is responsive at 500px such that your styles match the [mobile design file](design/Mobile.png).

### Task 2b: Minimum Viable Product - JavaScript

Navigate to `index.js` and complete the MVP challenges. Note that you need to scroll past data (or collapse data in VScode) to find the challenges below.



## Resources

📚[Best Practices for Responsive Design](https://www.browserstack.com/guide/responsive-design-breakpoints)

🤝[W3 Schools - Responsive Design](https://www.w3schools.com/html/html_responsive.asp)

👀 [Styling with HTML and CSS](https://www.w3schools.com/html/html_css.asp)

🦄 [Sprint Challenge Study Guide](https://www.notion.so/lambdaschool/Unit-1-Sprint-2-Study-Guide-16f656025c8744458addb068e6348101)


## Submission format

Please submit your project via codegrade by following [these instructions](https://www.notion.so/lambdaschool/Submitting-an-assignment-via-Code-Grade-A-Step-by-Step-Walkthrough-07bd65f5f8364e709ecb5064735ce374)


