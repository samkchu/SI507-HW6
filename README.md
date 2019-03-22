# JavaScript assignment

## Some useful resources
* Some [JavaScript tutorials](https://www.htmldog.com/guides/javascript/)
* The complicated [resources in the You Don't Know JS](https://github.com/getify/You-Dont-Know-JS) series, including [your reading last week](https://github.com/getify/You-Dont-Know-JS/blob/master/up%20%26%20going/ch2.md)
* [A resource for CSS/style/colors](https://htmlcolorcodes.com/)  
* [An excerpt from a specific workshop site](https://witny-summer-guild-2018.github.io/day_4_exercise_2.html) (for a different audience than yourselves) which addresses some common questions about jQuery
* [The simple JSFiddle example from class](https://jsfiddle.net/2of65j8q/)
* A [W3Schools resource on JavaScript output](https://www.w3schools.com/js/js_output.asp)
* Google, Piazza, your classmates, office hours, lab time!

## Included files
* This `README.md`, which you should edit with answers to the questions
* `jsPracticeLab.html`, which you'll need to edit and try out
* `jquerylib_submit_example.html`, which you'll need to edit and try out

## Your goals for this lab

### Broadly
The aim for this lab is to practice adapting to and understanding code in a new-to-you (or not) language and its own libraries/packages -- JavaScript, in this case.

The programming skills you have built up till now are useful for *Python programming*, but, more than that, they extend to fundamentals of many kinds of programming.

This experience is *not in any way* about becoming an expert JavaScript programmer. Instead, it is about using what you *do* have experience with -- and your skills in *learning new things* that relate to programming -- in order to make educated judgments about some brand new-to-you code, even if you haven't learned in detail about it yet. That's part of what being in technology -- or even technology-adjacent -- will often mean.

### Specifically

Below are a bunch of questions and indications of things to do. For each indication of something to do with code, there is also an accompanying question to answer or brief explanation to give.

**To complete and submit this assignment, you should:**

* Fork (and clone) this repository
* Add our instructional team as a collaborator to your fork (see instructions for adding collaborators on Canvas)
* Edit this `README.md` file with answers to the questions/prompts, briefly, using Markdown formatting so that the questions appear in bulletpoints and the answers appear clearly below each respective question, *not* as bulletpoints.
* Add all names of those who worked on this (as indicated below)
* Make the changes that are indicated below to each of the `.html` files with JavaScript programs provided. (You'll probably do this concurrently with answering questions)
* Commit (as you go) and push your changes to all three files to your GitHub forked repository.
* Submit a link to your repository on Canvas. (This HW doesn't have an autograder -- it will be graded by hand/by humans this time.)

### Important notes
* You are *more than* welcome to work together on this, but **you must <u>each</u> submit a repo to be graded on it**, so if you do work together, you should do the following:
	* Make sure each one of you understands all the work -- YOU are responsible for using and knowing this information
	* Write each person's name & uniqname who worked on the assignment together on your submitted `README.md` file (you'll see a space for this below)

* In answering questions, please make sure the formatting is clear to read and that you have updated the names of everyone who worked with you, with your name first (see below).

* In answering questions, assume all of the questions include a *explain briefly* note -- you do NOT have to, and should not, write extended paragraphs. Be as concise as you can and explain in your own words. Don't worry about "whether it's enough" -- just worry about conveying your understanding so you can read it later, or even give it to someone else, and the answers will help/make sense.

* It is not acceptable to copy and paste answers from the internet and submit them as your own. If you cite things, make sure you provide a citation, including to links. If you get information from a resource and rephrase it so you're basically explaining an idea, that's just fine for an explanatory purpose in this assignment, but you *must* cite any quotes or examples that aren't yours.

* **For grading:** we are grading on...
	* Following the instructions
	* Approximate correctness of the code edits
	* Careful & clear answers to the questions
	* Correct answers to the questions
	* Slightly more than half the 1000 points will come from answering the questions. The rest will come from your edits to the code.

### Names of people you have worked with on this assignment
* List everyone's names and uniqnames who have worked on this assignment with you, **including your own name, but make sure YOUR name is first and bold**
* Like this:
* **Jackie Cohen (jczetta)**
* Yea-Ree Chang (cyearee)
* Ruchi Ookalkar (ruchido)
* Innocent Obi (innoobi)
* Zhen Wang (alejwang)
* etc.

## Questions & code instructions

### The first questions address the `jsPracticeLab.html` file.

* **This is just an example question.**

This is what an example answer should look like. If you want to include some code, which you probably don't have to do, you can, like this:

```js
Some JavaScript code
```

* **What does a code comment look like in JavaScript? What character/s do you have to put before a comment?**

It looks like two /'s are how to input comments in JavaScript - so for example: `//this is a comment in JavaScript.`

* **Explain what needs to happen to get a JavaScript program to "run", given the JavaScript you've seen in this assignment.**

For this assignment, it appears to get the JavaScript to run, you have to open it in a web browser - this executes not just the JavaScript, but also the HTML and CSS code.

* **What functions in JavaScript seem to be similar in function to the `print` function in Python? (There are two.) Why might you use one and not the other? Explain briefly.**

In this code, two ways of displaying text to a user appears to be the `innerhtml()` "method" and `alert()` method. The `innerhtml()` method seems to display things in the browser output, whereas the `alert()` method displays things in a pop-up alert. `innerhtml()` would be useful for manipulating the actual page, whereas `alert()` would be useful to a certain type of event, triggered by a user action.

* **What code would have to comment out to get rid of the pop-up box when you load the page? (Related to the last question.) Do that in the code file, and then, add code so that a text box will appear that contains the current date and time! *HINT:* Look through the rest of the code first...**

You should comment out line 12. To add an alert that contains today's date, we can use a similar syntax, but instead of the string `hello` we can insert the code `new Date()`.

* **How can you put your own name at the top where it currently says "A name"? Explain very briefly how to do so, and replace `A name` in the web page with your own name.**

You can replace the string in `document.querySelector('h1').innerHTML = "A name";` with your own name. So, instead: `document.querySelector('h1').innerHTML = "Samantha Chu";`.

* **What does the word `document` represent in this code? Explain briefly.**

`document` seems to represent an object; more specifically, it seems to represent the overall webpage. When we use a method on this object, for example `querySelector()`, we are finding and selecting a query within the `document` object.

* **What is happening in line 12 (
		`document.querySelector('#items').innerHTML = document.getElementsByTagName('li').length`
)? Explain, briefly (<= 2 sentences).**

It appears that the code is finding the elements in the webpage that are in a list format (i.e. tagged through the `<li>` HTML tag) and "counting" them using a `length()` method. It then assigns this count value to the object marked `#items`, which is displayed on the webpage.

* **What color would the background of this page be <u>if there were no JavaScript in this page</u>?**

It would be white.

* **Why are there a couple of gray boxes on the screen with a different colored border? How could you edit this code to make them a different color? Explain briefly. Then edit the code to make those boxes some shade of blue, of your choosing.**

There are "boxes" because in the CSS portion of the code, the CSS "tells" the webpage that any `<p>` (paragraph) tagged HTML should have a gray background color and a solid, colored border. We can edit this particular CSS code to make the paragraphs a different color, such as #496aed.

* **Edit the code so that, if you highlight `McGill University` and copy it, you see the text `O Canada` near the bottom of the page. Briefly explain why you made the edits that you did -- how did you know/figure out what to do?**

I looked at the `copyFunction()` that acted upon the `University of Michigan` string - I noticed that the `copyFunction()` added additional text to the lowest portion of the webpage (marked by a `div` tag). In the `<li>` tag for `University of Michigan`, the syntax `oncopy` specified what should happen if a user uses the keyboard shortcut to copy this text, that is, the `copyFunction()` should be invoked.

I wrote similar code for the `McGill University` by adding a second function and a second tag, which returns `0 Canada` near the bottom of the page if `McGill University` is acted upon by Ctrl+C.

* **In the original code, when you click the button that says `Wow`, you see a text box! Wow. Explain briefly in your own words why the following code causes that to happen:**

```js
function handleClick(){
	alert("hello");
}
```

**and**

```js
<button onclick=handleClick() id="wow-button">Wow</button>
```

The first bit code defines a function called `handleClick`, which returns an alert text box displaying the string `hello` when invoked.

The second bit of code says that when this button is clicked, invoke the `handleClick()` function.

Together, if/when a user clicks on the button, it invokes the `handleClick()` function, which returns an alert text box.


* **Knowing what you learned from the previous question, add code/markup to the `jsPracticeLab.html` file *so that* there is a button with the text `Spring Equinox 2019` on it somewhere on the page, and when that button is clicked, a text box containing the text `March 20, 2019` appears. (There's no function -- that I am aware of -- to automatically get this info, you've got to type it yourself.)**

See file.

### The next few questions address the `jquerylib_submit_example.html` file.

* **Check out the file `jquerylib_submit_example.html`. This is an example of code that uses a package called `jQuery` (and this will need you to have an internet connection to run it properly, although the other file does not). Check out resources above for more on jQuery!**

* **When you enter input that isn't valid, you see an error that is red. Why is the error in red? Why is the response for valid inputs blue?**

The error is in red because an invalid input results in a `<p>` object tagged with the class `"error"`. The CSS code says that this object should be colored red. On the contrary, valid inputs are blue because the resulting `<p>` object is tagged as class `"good"`, which the CSS code says to be colored blue.

* **What is this line `var regex = /^[a-zA-Z]+$/;` helping with? And if you googled something to figure that out, what did you google, and what, briefly, did you learn? (If you didn't need to google, you can leave that out, but explain briefly what that line is helping the program do, anyway.)**

The line `var regex = /^[a-zA-Z]+$/` is helping create a test for the user input. It represents a valid input - that is, one word, with no spaces. I googled around for the meaning of "var regex" and found a blog post that helped describe Regular Expressions and their syntax: "A Practical Guide to Regular Expressions (RegEx) in JavaScript" by Sukhjinder Arora (found here: https://blog.bitsrc.io/a-beginners-guide-to-regular-expressions-regex-in-javascript-9c58feb27eb4). I learned that these "Regular Expressions" can help describe conditions/patterns for strings.

* **What's different about the syntax of conditional statements in JavaScript, compared to Python?**

It seems that each "rule" of the conditional is contained by `{ }` brackets. Also, every line of code within these brackets must end with `;`.

* **What do you think the `10000` refers to in the code `.fadeOut(10000)`?**

I think it refers to something to do with the behavior of how the string "fades" away. After testing different inputs, it looks like it controls the speed of the fading away.

* **What do you think is going on with the following code at the beginning of the program? Note that the most important thing to do for answering this question is to be thoughtful and clear, not to be absolutely correct:**

```js
$(document).ready(function(){
    $("form").submit(function(event){
```

I think it has something to do with telling the JavaScript code to run upon the the event of a user clicking submit. The initial display (that a user sees on the webpage) relies on HTML; however, for the "logic" of the webpage to work, the JavaScript conditional has to be triggered somehow. I think this is what that code is for.

* **Add some code to the `jquerylib_submit_example.html` file so that, if the input is valid and is specifically the text `hello`, rather than the visible output being `Nice!` in blue, the visible output should be `Hello to you too!`, also in blue, just like `Nice!` is.**
	* *HINT:* You'll have to make some changes to the conditional statement, and possibly look up some JavaScript conditional syntax. You'll also need to look carefully at what generates visible output right now.
