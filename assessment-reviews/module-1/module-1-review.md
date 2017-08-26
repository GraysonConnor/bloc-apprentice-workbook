# Module 1 Review Questions and Exercises

## Instructions

1. Click "edit" at the top of the page.
2. Fill in your answers below each question.
3. Save your changes and send a link to your mentor!

## HTML

### Questions

1. What is HTML and what is it used for?
HyperText Markup Language is a text-based language that is translated by a web browser in order to display content.

2. What is the difference between an ID and a class? A class atribute is usually used on multiple elements in your HTML. An ID tribute identifies a unique element in your HTML.

3. What does it mean to write "semantic" HTML? 
Semantic HTML communicates the meaning, purpose, or context of the code instead of just the presentation.

### Exercises

1. Write a paragraph tag with a class of "highlight" and content "Watch out!".
<p class="highlight">"Watch out!"</p>

2. Write an HTML image tag to show an image called `profile-picture.jpg`.
  <img src="profile-picture.jpg">

3. Write a link tag that links to http://google.com.
<a href="http://google.com">

5. Write an complete standard HTML document outline (including a DOCTYPE, and `<html>`, `<head>`, and `<body>` tags).
<!DOCTYPE html>
<html>
<head>
</head>
<body>
</body>
</html>

6. Inside of the code for the previous exercise, write the appropriate tag to link to a script file called `main.js`.
<html>
  <head>
    <script type="text/javascript" src="main.js"></script>
  </head>
	<body>
	</body>
</html>

7. Inside of the code for the previous exercise, write the appropriate tag to link to a stylesheet file called `main.css`.
<link rel="stylesheet" href="styles.css">

8. Write a numbered list in HTML and list three of your favorite books.
  <ol>
    <li>Harry Potter: Order of the Phoenix</li>
    <li>Harry Potter: Goblet of Fire</li>
    <li>Harry Potter: Half Blood Prince</li>
  </ol> 

9. Fix the indentation of the following HTML sample:

  ```html
<div>
  <ul>
    <li>Item 1</li>
    <li>Item 2</li>
    <li>Item 3</li>
  </ul>
</div>
  ```

## CSS

### Questions

1. What is CSS and what is it used for?
Cascading Style Sheets and it is used to apply ascetics and formation to your html.

2. What is the CSS box model?
The box model is essentially a box that is wrapped around your html content. It is made up of borders, margins, padding, and your actual content.

3. What's the difference between margin and padding?
Padding clears an area around the content. Margin clears an area outside the border. Both are transparent.

### Exercises

1. Write a CSS rule to make the text of all `h1` tags red.
h1 {
color: red;
}

2. Write a CSS rule to make the background color of the link with `class="btn"` blue:

.btn {
background-color: blue;
}
  ```html
  <a href="#" class="btn">Learn more</a>
  ```

3. Write a CSS rule to give the first paragraph in the following HTML a font size of `20px`, but not the second paragraph.
.jumbotron p {
font-size: 20px;

  ```html
  <header class="jumbotron">
    <p>Hello, World!</p>
  </header>

  <p>Welcome to this awesome website!</p>
  ```

## JavaScript

### Questions

1. What is a function? What are they used for?
A JavaScript function is a block of code designed to perform a particular task.

2. What is the difference between `==` and `===`?
 ***The identity (===) operator behaves identically to the equality (==) operator except no type conversion is done.*** (Copied this one from the internet)

3. What is the difference between global and local scope variables? A local scope variable is a variable that will only be active within a specified function. A global scope variable will affect several elements.

4. What is a boolean value?
 A Boolean value represents two values, either "true" or "false". 

5. What is an array?
An array is a variable which can hold more than one value at a time.

### Exercises

1. Write a line that declares a variable called `myName` and set its value to your name.
var myName="Grayson"

2. Write a loop that logs the numbers 1 through 10 to the console.
var num=1
while(num<=10){
  console.log(num);
  num++
}

3. Translate the following pseudocode into JavaScript: if `score` is greater than `3` and `lives` is greater than `0`, alert "You win!".

if(score>3 && lives>0){
alert("You win!");
}


4. Write a function `sayHello` that takes one argument, a name, and logs "Hello, <name>!" to the console. Then, call the function below the function definition and pass in your name as the argument.
	function sayHello(name){
	
	console.log("Hello, "+name+"!");
	}
	
	sayHello(Grayson);
	
5. What would the following script log to the console?

  ```javascript
  var currentSong = "Call Me Maybe";

  function setSong(song) {
    currentSong = song;
  }

  setSong("Friday, Friday");

  console.log(currentSong);
  ```
"Call me Maybe"

6. What would the following script log to the console?

  ```javascript
  var add = function(a, b) {
    return a + b;
  }

  var result = add(3, 7);

  console.log(result);
  ```10

7. What would the following script log to the console?

  ```javascript
  var helloGoodbye = function(name) {
    return sayHello(name) + " " + sayGoodbye(name);
  }

  var sayHello = function(name) {
    return "Hello " + name " !";
  }

  var sayGoodbye = function(name) {
    return "Goodbye " + name " !";
  }

  console.log(helloGoodbye("Sarah"));
  ```Hello Sarah! Goodbye Sarah!

8. Write a function `findLongestWord()` that takes an array of words and returns the length of the longest one.
var findLongestWord = ["green", "blue", "purple"];
var largest = 0;
for (var i = 0; i < findLongestWord.length; i++) {
    if (findLongestWord[i].length > largest) {
        largest = findLongestWord[i].length;
    }
}
console.log(largest);

9. Define a function `sum()` that sums all the numbers in an array of numbers. For example, `sum([1,2,3,4])` should return 10.

function sum([a,b,c]){
console.log(a+b+c); 
}
sum([4,7,18]);

10. Write a function that takes a character (i.e. a string of length 1) and returns true if it is a vowel, false otherwise.
function vowel(string){
  if(string=="a","e","i","o","u","y"){
    console.log("true")
  }else{
    console.log(false)  
  }
}
vowel(string);

11. Write the correct line to make `"Woof!"` show up in the console based on this script:

  ```javascript
  var pet = {
    name: "Charles",
    goodDog: true,
    speak: function() {
      console.log("Woof!");
    }
  };
  ```pet.speak();

12. Using the same script as above, write the correct line to log the dog's name to the console.
console.log(pet.name)
## Command Line

### Questions

1. What is the command line and what is it used for?
The command line is a text based user interface that allows you to issue commands to your computer using only text.

2. What does the command `ls` do?
"ls" will list all files.

3. What does the command `pwd` do?
"pwd" will print the working directory.

4. What does the following command do: `cd my-cool-project`
Change the working directory to my-cool-project.

### Exercises

1. Write the command to make a new directory called "my-cool-project".
mkdir my-cool-projects

2. Write the command to create a file called "index.html".
touch index.html

3. Write the command to delete a file called "main.css".
rm main.css

## Git

### Questions

1. What is Git and what is it used for?
 Git is a distributed version control system, and it allows multiple people to work on and share the same project.

2. What's the difference between a local repository and a remote repository?
A local directory is located on an users computer. A remote directory is one located on a different server such as github.

### Exercises

1. Write the command that you would use to create a new local Git repository.
git init

2. Write the command to stage a file called `index.html` to be committed.
add index.html

3. Write the command to view the current status of the git repository.
git status
