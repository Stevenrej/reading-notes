# Reading Notes 2

## HTML Text Fundamentals

Description lists
In HTML text fundamentals, we walked through how to mark up basic lists in HTML, but we didn't mention the third type of list you'll occasionally come across — description lists. The purpose of these lists is to mark up a set of items and their associated descriptions, such as terms and definitions, or questions and answers. Let's look at an example of a set of terms and definitions:

soliloquy
In drama, where a character speaks to themselves, representing their inner thoughts or feelings and in the process relaying them to the audience (but not to other characters.)
monologue
In drama, where a character speaks their thoughts out loud to share them with the audience and any other characters present.
aside
In drama, where a character shares a comment only with the audience for humorous or dramatic effect. This is usually a feeling, thought or piece of additional background information
Description lists use a different wrapper than the other list types — <dl>; in addition each term is wrapped in a <dt> (description term) element, and each description is wrapped in a <dd> (description definition) element.

Description list example
Let's finish marking up our example:

<dl>
  <dt>soliloquy</dt>
  <dd>In drama, where a character speaks to themselves, representing their inner thoughts or feelings and in the process relaying them to the audience (but not to other characters.)</dd>
  <dt>monologue</dt>
  <dd>In drama, where a character speaks their thoughts out loud to share them with the audience and any other characters present.</dd>
  <dt>aside</dt>
  <dd>In drama, where a character shares a comment only with the audience for humorous or dramatic effect. This is usually a feeling, thought, or piece of additional background information.</dd>
</dl>

Abbreviations
Another fairly common element you'll meet when looking around the Web is <abbr> — this is used to wrap around an abbreviation or acronym. When including either, provide a full expansion of the term in plain text on first use, along with the <abbr> to mark up the abbreviation. This provides a hint to user agents on how to announce/display the content while informing all users what the abbreviation means.

If providing the expansion in addition to the abbreviation makes little sense, and the abbreviation or acronym is a fairly shortened term, provide the full expansion of the term as the value of title attribute:

Abbreviation example
Let's look at an example.

<p>We use <abbr>HTML</abbr>, Hypertext Markup Language, to structure our web documents.</p>

<p>I think <abbr title="Reverend">Rev.</abbr> Green did it in the kitchen with the chainsaw.</p>

Superscript and subscript
You will occasionally need to use superscript and subscript when marking up items like dates, chemical formulae, and mathematical equations so they have the correct meaning. The <sup> and <sub> elements handle this job. For example:

<p>My birthday is on the 25<sup>th</sup> of May 2001.</p>
<p>Caffeine's chemical formula is C<sub>8</sub>H<sub>10</sub>N<sub>4</sub>O<sub>2</sub>.</p>
<p>If x<sup>2</sup> is 9, x must equal 3 or -3.</p>



1. So a reader of the code can easily make sense of it. Search engines and assisitive technologies also are helped by using semantic elements.

2. There are six levels of headings in html

3. These elements allow you to use superscript and subscript to easliy display information

4. Title= must be added

## How CSS is structured 

Transform functions
Another example would be the various values for transform, such as rotate().

<div class="box"></div>
Copy to Clipboard
.box {
  margin: 30px;
  width: 100px;
  height: 100px;
  background-color: rebeccapurple;
  transform: rotate(0.8turn);
}

@rules
CSS @rules (pronounced "at-rules") provide instruction for what CSS should perform or how it should behave. Some @rules are simple with just a keyword and a value. For example, @import imports a stylesheet into another CSS stylesheet:

@import 'styles2.css';
Copy to Clipboard
One common @rule that you are likely to encounter is @media, which is used to create media queries. Media queries use conditional logic for applying CSS styling.

In the example below, the stylesheet defines a default pink background for the <body> element. However, a media query follows that defines a blue background if the browser viewport is wider than 30em.

body {
  background-color: pink;
}

@media (min-width: 30em) {
  body {
    background-color: blue;
  }
}
Copy to Clipboard
You will encounter other @rules throughout these tutorials.

See if you can add a media query that changes styles based on the viewport width. Change the width of your browser window to see the result.




1. Through an external style sheet, internal style sheet and inline in the html

2. It is the least effective way of using CSS for maintenance and secondly it can mess with the presentation of the html code which can make it more difficult to read and understand

3. 
- h2 is representing the selector
- color and padding are part of the css declaration
- the properties are black and 5px

## JavaScript Basics

Operators
An operator is a mathematical symbol that produces a result based on two values (or variables). In the following table, you can see some of the simplest operators, along with some examples to try in the JavaScript console.

Operator	Explanation	Symbol(s)	Example
Addition	Add two numbers together or combine two strings.	+	6 + 9;
'Hello ' + 'world!';
Subtraction, Multiplication, Division	These do what you'd expect them to do in basic math.	-, *, /	9 - 3;
8 * 2; // multiply in JS is an asterisk
9 / 3;
Assignment	As you've seen already: this assigns a value to a variable.	=	let myVariable = 'Bob';
Strict equality	This performs a test to see if two values are equal. It returns a true/false (Boolean) result.	===	let myVariable = 3;
myVariable === 4;
Not, Does-not-equal	This returns the logically opposite value of what it precedes. It turns a true into a false, etc.. When it is used alongside the Equality operator, the negation operator tests whether two values are not equal.	!, !==	
For "Not", the basic expression is true, but the comparison returns false because we negate it:

let myVariable = 3;
!(myVariable === 3);

"Does-not-equal" gives basically the same result with different syntax. Here we are testing "is myVariable NOT equal to 3". This returns false because myVariable IS equal to 3:

let myVariable = 3;
myVariable !== 3;

There are a lot more operators to explore, but this is enough for now. See Expressions and operators for a complete list.

Events
Real interactivity on a website requires event handlers. These are code structures that listen for activity in the browser, and run code in response. The most obvious example is handling the click event, which is fired by the browser when you click on something with your mouse. To demonstrate this, enter the following into your console, then click on the current webpage:

document.querySelector('html').addEventListener('click', function () {
  alert('Ouch! Stop poking me!');
});
Copy to Clipboard
There are many ways to attach an event handler to an element. Here we select the <html> element. We then call its addEventListener() function, passing in the name of the event to listen to ('click') and a function to run when the event happens.

1. that would be considered a string variable

2. 4 diffrent javascript operators are Addition, Assignment, strict equality and does not equal

3. Simply you can use functions to make a calculator but at most you could use functions to help with countless issues 

## Conditionals

if...else statements
Let's look at by far the most common type of conditional statement you'll use in JavaScript — the humble if...else statement.

Basic if...else syntax
Basic if...else syntax looks like this:

if (condition) {
  /* code to run if condition is true */
} else {
  /* run some other code instead */
}
Copy to Clipboard
Here we've got:

The keyword if followed by some parentheses.
A condition to test, placed inside the parentheses (typically "is this value bigger than this other value?", or "does this value exist?"). The condition makes use of the comparison operators we discussed in the last module and returns true or false.
A set of curly braces, inside which we have some code — this can be any code we like, and it only runs if the condition returns true.
The keyword else.
Another set of curly braces, inside which we have some more code — this can be any code we like, and it only runs if the condition is not true — or in other words, the condition is false.
This code is pretty human-readable — it is saying "if the condition returns true, run code A, else run code B"

You should note that you don't have to include the else and the second curly brace block — the following is also perfectly legal code:

if (condition) {
  /* code to run if condition is true */
}

/* run some other code */
Copy to Clipboard
However, you need to be careful here — in this case, the second block of code is not controlled by the conditional statement, so it always runs, regardless of whether the condition returns true or false. This is not necessarily a bad thing, but it might not be what you want — often you want to run one block of code or the other, not both.

As a final point, while not recommended, you may sometimes see if...else statements written without the curly braces:

if (condition) /* code to run if condition is true */
else /* run some other code instead */
This syntax is perfectly valid, but it is much easier to understand the code if you use the curly braces to delimit the blocks of code, and use multiple lines and indentation.

else if
The last example provided us with two choices, or outcomes — but what if we want more than two?

There is a way to chain on extra choices/outcomes to your if...else — using else if. Each extra choice requires an additional block to put in between if () { } and else { } — check out the following more involved example, which could be part of a simple weather forecast application:

<label for="weather">Select the weather type today: </label>
<select id="weather">
  <option value="">--Make a choice--</option>
  <option value="sunny">Sunny</option>
  <option value="rainy">Rainy</option>
  <option value="snowing">Snowing</option>
  <option value="overcast">Overcast</option>
</select>

<p></p>
Copy to Clipboard
const select = document.querySelector('select');
const para = document.querySelector('p');

select.addEventListener('change', setWeather);

function setWeather() {
  const choice = select.value;

  if (choice === 'sunny') {
    para.textContent = 'It is nice and sunny outside today. Wear shorts! Go to the beach, or the park, and get an ice cream.';
  } else if (choice === 'rainy') {
    para.textContent = 'Rain is falling outside; take a rain coat and an umbrella, and don\'t stay out for too long.';
  } else if (choice === 'snowing') {
    para.textContent = 'The snow is coming down — it is freezing! Best to stay in with a cup of hot chocolate, or go build a snowman.';
  } else if (choice === 'overcast') {
    para.textContent = 'It isn\'t raining, but the sky is grey and gloomy; it could turn any minute, so take a rain coat just in case.';
  } else {
    para.textContent = '';
  }
}

A note on comparison operators
Comparison operators are used to test the conditions inside our conditional statements. We first looked at comparison operators back in our Basic math in JavaScript — numbers and operators article. Our choices are:

=== and !== — test if one value is identical to, or not identical to, another.
< and > — test if one value is less than or greater than another.
<= and >= — test if one value is less than or equal to, or greater than or equal to, another.

Logical operators: AND, OR and NOT
If you want to test multiple conditions without writing nested if...else statements, logical operators can help you. When used in conditions, the first two do the following:

&& — AND; allows you to chain together two or more expressions so that all of them have to individually evaluate to true for the whole expression to return true.
|| — OR; allows you to chain together two or more expressions so that one or more of them have to individually evaluate to true for the whole expression to return true.
To

switch statements
if...else statements do the job of enabling conditional code well, but they are not without their downsides. They are mainly good for cases where you've got a couple of choices, and each one requires a reasonable amount of code to be run, and/or the conditions are complex (for example, multiple logical operators). For cases where you just want to set a variable to a certain choice of value or print out a particular statement depending on a condition, the syntax can be a bit cumbersome, especially if you've got a large number of choices.

In such a case, switch statements are your friend — they take a single expression/value as an input, and then look through a number of choices until they find one that matches that value, executing the corresponding code that goes along with it. Here's some more pseudocode, to give you an idea:

switch (expression) {
  case choice1:
    run this code
    break;

  case choice2:
    run this code instead
    break;

  // include as many cases as you like

  default:
    actually, just run this code
}
Here we've got:

The keyword switch, followed by a set of parentheses.
An expression or value inside the parentheses.
The keyword case, followed by a choice that the expression/value could be, followed by a colon.
Some code to run if the choice matches the expression.
A break statement, followed by a semi-colon. If the previous choice matches the expression/value, the browser stops executing the code block here, and moves on to any code that appears below the switch statement.
As many other cases (bullets 3–5) as you like.
The keyword default, followed by exactly the same code pattern as one of the cases (bullets 3–5), except that default does not have a choice after it, and you don't need to break statement as there is nothing to run after this in the block anyway. This is the default option that runs if none of the choices match.
Note: You don't have to include the default section — you can safely omit it if there is no chance that the expression could end up equaling an unknown value. If there is a chance of this, however, you need to include it to handle unknown cases.

A switch example
Let's have a look at a real example — we'll rewrite our weather forecast application to use a switch statement instead:

<label for="weather">Select the weather type today: </label>
<select id="weather">
  <option value="">--Make a choice--</option>
  <option value="sunny">Sunny</option>
  <option value="rainy">Rainy</option>
  <option value="snowing">Snowing</option>
  <option value="overcast">Overcast</option>
</select>

<p></p>
Copy to Clipboard
const select = document.querySelector('select');
const para = document.querySelector('p');

select.addEventListener('change', setWeather);

function setWeather() {
  const choice = select.value;

  switch (choice) {
    case 'sunny':
      para.textContent = 'It is nice and sunny outside today. Wear shorts! Go to the beach, or the park, and get an ice cream.';
      break;
    case 'rainy':
      para.textContent = 'Rain is falling outside; take a rain coat and an umbrella, and don\'t stay out for too long.';
      break;
    case 'snowing':
      para.textContent = 'The snow is coming down — it is freezing! Best to stay in with a cup of hot chocolate, or go build a snowman.';
      break;
    case 'overcast':
      para.textContent = 'It isn\'t raining, but the sky is grey and gloomy; it could turn any minute, so take a rain coat just in case.';
      break;
    default:
      para.textContent = '';
  }
}
Copy to Clipboard


1. An if statement checks a condition and if it evaluates to true, then the code block will execute.

2. else if is used if there are multiple options/answers. You would put else if after an if statement and and before and else statement

3. Three diffrent comparison operators could be ===, < or <=

4. && stand for AND which means if you put this in your code both expresions would have to be true for the code to execute while || stands for OR which means if one of the two expresions is true the code will execute



 [Back To 201 Notes](https://stevenrej.github.io/reading-notes/readingnotes201main)