# 100 Days Of Code - Log

### Day 1: January 1st, 2017


**Today's Progress**: Completed JS30 challenge 1

**Thoughts/Learned something new:**

   
    (HTML) data-* attribute. I can call my data attribute whatever I want. Example: data-banana, data-hello, data-foo
    (HTML) <audio src="something.wav"></audio> embeds sounds in HTML that can be referenced
    (HTML) <kbd></kbd> adds font aesthetic/styling and references keyboard input.
    (JS) The querySelector() method returns the first element that matches a specified CSS selector(s) or HTML tag in the document.
    (JS) The addEventListener() method attaches an event handler to the specified element. http://www.w3schools.com/jsref/dom_obj_event.asp
    (JS)/(CSS) http://www.w3schools.com/css/css_attribute_selectors.asp 
    (JSES6) Backticks `` allow insertion of variables into strings ${variablenamehere}
    (Jquery/ JS) key.addClass('playing') same as key.classList.add("playing');
    (CSS)_transition/transform relationship
    (JS) querySelectorAll(".class") returns all the matches and places them in a Nodelist that acts like an array
    (JS) transitionend (Transition End) is an event listener event
    (JS) The forEach() method calls a provided function once for each element in an array, in order.

   Note to self: Review notes periodically in file


**Link to work:** See Day 1 Drum Kit folder

### Day 2: January 2nd, 2017


**Today's Progress**: Completed freecodecamp algorithm challenge "Return largest numbers in Arrays"
Deleted Repo since contributions weren't showing on fork. Restarted as owner

**Thoughts/Learned something new:**

   I was given a 2D array and asked to return the largest number in each array using a function. The exercise suggested I use comparison operators, but for my initial attempt I used a for loop that iterates through each array and sorts them from least to greatest using the sort() array method. The sort() method has to take a function to sort numbers, as it really only sorts strings by default. Then I used the pop() method to remove the last (largest) number in the now sorted array. I used the push() method to add it to a new array. I then returned the newArray. Since FCC runs multiple function argument tests, I realized that each time the function ran, my newArray would keep getting larger. I moved my var newArray = [] declaration from global scope to inside the function. Everytime the function runs, the newArray would be reset (emptied).

 

**Link to work:** 
https://www.freecodecamp.com/challenges/return-largest-numbers-in-arrays

function largestOfFour(arr) {

  var newArray = [];

  for (i = 0; i < arr.length; i++){
  arr[i].sort(function(a, b){
    return a-b;
  });
  
  var number = arr[i].pop();
  
  newArray.push(number);
  }

  return newArray;
  
}

largestOfFour([[13, 10000, 18, 26], [4, 5, 1, 3], [32, 35, 37, 39], [1000, 1001, 857, 1]]);


### Day 3: January 3rd, 2017


**Today's Progress**: Completed a FizzBuzz challenge and ready 2 chapters of Eloquent Javascript

**Thoughts/Learned something new:**
There is a Number() function that is similar (but different) to parseInt()


ternary operator. If condition is true, middle thing is chosen, otherwise the last item is chosen
console.log(CONDITION ? MIDDLETHING : LASTTHING);
console.log(true ? 1 : 2);
// → 1
console.log(false ? 1 : 2);
// → 2

   

**Link to work:** 

for (i = 1; i <= 100; i++){
	if(i % 15 === 0){
  console.log("FizzBuzz");
  } else if(i % 5 === 0){
  console.log("Buzz");
  } else if(i % 3 === 0){
  console.log("Fizz");
  } else{
  console.log(i);
  }
}


### Day 4: January 4th, 2017


**Today's Progress**: Worked on a CSS/Javascript clock

**Thoughts/Learned something new:**
Used some ECMA6 techniques again: const and backtick string stuff: `${variable}`
(CSS) transform: rotate(180deg);
(CSS) transition
(CSS) transition-timing-function
(CSS) transform-origin: defaults to start animation at 50%, had to change it to 100% (far right)
(JS) document.querySelector(".class"); [review]
(JS) Variety of Date() object
var now = new Date(); //constructor
var seconds = now.getSeconds(); //call method of date object to get the current time in seconds


   

**Link to work:** 

See Day 2 JS + CSS Clock


### Day 5: January 5th, 2017 SNOWDAY!!!


**Today's Progress**: Completed another FizzBuzz exercise and a solution to a checkerboard algorithm. Read Chapter 3 of Eloquent Javascript

**Thoughts/Learned something new:**

   

**Link to work:**
Checkerboard solution

finString = "";
space = " ";
hash = "#";
size = 8;
newLine = "\n";

for(j = 0; j < size; j++){

    for(i = 0; i < size; i++){
        if(i % 2 === 0){
            finString += space;
        }else{
            finString += hash;
        }
       
	}
 finString += newLine;
}
console.log(finString);
    


### Day 6: January 6th, 2017 SNOW DAY!!


**Today's Progress**: Completed a nested scope example and shared it will the class. Created a very basic "Yoda Speak" API call using Jquery/Ajax

**Thoughts/Learned something new:**
I spent who knows how long trying to figure out why my API calls weren't working only to find that the server was down, you never know!
I'm really taking some time to learn closure and recursion, I'll of course need to return to these topics.
   

**Link to work:** 
See repo yodaspeak


### Day 7: January 7th, 2017


**Today's Progress**: Reviewed some Javascript and jQuery on codeacademy and teamtreehouse. Looked over some items on LinkedIn to see what is out there. Felt a little under the weather, but tried to get some work done.

**Thoughts/Learned something new:**
I'm realizing that only coding multiple projects is going to help me remember/recall the major syntax items I'll be using in my career. Everything else I can look up when needed. Sublime snippets help.
   

**Link to work:** none


### Day 8: January 8th, 2017


**Today's Progress**: Built a basic plan for my Trivia Game (Simpsons themed), coded out a framework. Reviewed Jon Duckett Javascript/Jquery

**Thoughts/Learned something new:**
Really felt like I helped build on some of the jQuery and Javascript items I was having trouble recalling after reviewing the Duckett book. I placed some markets on some key pages that have some good resources.

   

**Link to work:**  None posted


### Day 9: January 9th, 2017


**Today's Progress**: Scrapped yesterday's work. Completed a Trivia Game assignment from start to finish.

**Thoughts/Learned something new:**
Used lots of jQuery
Implemented an Array of Objects
Used object constructors
Used different javascript timers
Used a CSS animation
I will want to look over this project again to try to optimize it. I'm not sure my object calls are more efficient.
Ordered The Little Schemer, I read that it's good for conceptually understanding programming recursion
Threw in a jQuery UI starter animation

**Link to work:** 
see folder Trivia Game

### Day 10: January 10th, 2017


**Today's Progress**: stuck in the driveway yesterday and missed class, I made up my class today after work. We built most of our New York Times API's app in a group project

**Thoughts/Learned something new:**
Felt pretty comfortable on the backend with the AJAX calls
Would like to review Bootstrap seeing how fast a team member put the front-end site together!

   

**Link to work:** Should be a forked repository about a New York Times App


### Day 11: January 11th, 2017


**Today's Progress**: Learned about localStorage, sessionStorage, cookies

**Thoughts/Learned something new:**
Had a pretty difficult class exercise that we worked on in groups at the end of class using localStorage.
I enjoyed the challenge. We were close to the solution, but did not finish. I want to try to complete this challenge soon.   

**Link to work:** Not pushed to GitHub yet.



### Day 12: January 12th, 2017


**Today's Progress**: Restructuring a new study plan to try to loosely stick to. It's an 8 hour outline that I will not always be able to complete, but it's designed to keep me building and learning on a regular schedule.

**Thoughts/Learned something new:**
Refreshed my memory on:
document.getElementByID;
addEventListener
Seems that using jQuery for a while can mess my JavaScript memory up
Completed 2 algorithms, and offered to help someone online without a response from them,
Reviewed some basic loop structures on CodeAcademy, and then began a small project in JSBin

**Link to work:** 

function confirmEnding(str, target) {
  
  var lastLetter = str.substring(str.length - target.length);
  if(target === lastLetter){
    return true;
  } else{
    return false;
  }
}

confirmEnding("Bastian", "n");

//

function repeatStringNumTimes(str, num) {
    var holdvar = "";
    for(i = 0; i < num; i++){
    
    holdvar += str;
    }
    return holdvar;
}

repeatStringNumTimes("abc", 3);



### Day 13: January 13th, 2017 Day 0 of flu!


**Today's Progress**:

code academy, messing around in JSBin. Created a basic dragon attack text based game based on random chance.

**Thoughts/Learned something new:**
Problem solving practice
Review of do while loops
   

**Link to work:** 

function truncateString(str, num) {
  // Clear out that junk in your trunk
  if(num >= str.length){
    return str;
  }else if (num <= 3){
    str = str.slice(0, num) + "...";
  return str;
  }else {
    str = str.slice(0, num -3) + "...";
    return str;
  }
}

truncateString("A-tisket a-tasket A green and yellow basket", 11);
//

function chunkArrayInGroups(arr, size) {
  // Break it up.
    var arr2 = [];
    var i = 0;
      while(i < arr.length){
      var sliced = arr.slice(i, i + size);  
      arr2.push(sliced);
      i += size;
      }

    return arr2;

}

chunkArrayInGroups([0, 1, 2, 3, 4, 5], 3);

### Day 14: January 14th, 2017 Day 1 of flu!


**Today's Progress**: 
Solved 2 algorithms. Code academy, messed about in JSBin again. Did Khan academy. 

**Thoughts/Learned something new:**
Created different things in Firebase. Firebase allows me to access a server side database to update information live on the page without refresh, multiple people accessing the page can change the results.

**Link to work:** 

function slasher(arr, howMany) {
  return arr.slice(howMany);

}

slasher([1, 2, 3], 2);
//

function mutation(arr) {
  var firstWord = arr[0].toLowerCase();
  var secondWord = arr[1].toLowerCase();
 

  
  for(i = 0; i < secondWord.length; i++){
    if (firstWord.indexOf(secondWord[i]) === -1){
      return false;
    } 
    
  }
  return true;
}
 

mutation(["hello", "hey"]);



### Day 15: January 15th, 2017 Day 2 of flu!

**Today's Progress**:
Code Academy JS, messed about in JSbin some. Did day 4 of JS30. Created a slider toggle for 3 different settings to alter the CSS properties of an image.

**Thoughts/Learned something new:**
CSS variables!??!
Arrow function review

**Link to work:** 

see JS30 repo


### Day 16: January 16th, 2017 Day 3 of flu!


**Today's Progress**:
Completed giphy api search homework from start to finish

**Thoughts/Learned something new:**
reviewed Ajax calls using jquery
used figure and figcaption HTML
reviewed bootstrap classes
used some fontawesome icons
took a while to find a bug...missing a colon!

**Link to work:** 
see repo GiphyApp




### Day 17: January 17th, 2017 Day 4 of flu!


**Today's Progress**:
Worked on my RPG game during a extra help day. Figured out the basic logic required to complete the game

**Thoughts/Learned something new:**
calling scoped items through window["object"].key
Putting objects within an object to keep them outside of global scope (global scope is bad practice!);

**Link to work:** 


var characters = {

	 batman: new Character("Batman", "batman"),
	 superman: new Character("Superman", "superman"),
	 joker: new Character("Joker", "joker"),
	 lexLuthor: new Character("Lex Luthor", "lexLuthor")

 
}



### Day 18: January 18th, 2017 Day 5 of flu!


**Today's Progress**:
Worked in groups for New York Times app and built an employee tracker in teams

**Thoughts/Learned something new:**
More exposure to firebase database and practice using Bootstrap

**Link to work:** 

employee tracker commits with forks


### Day 19: January 19th, 2017


**Today's Progress**:
Worked on adding objects to hangman game, still did not turn the game into a complete object.

**Thoughts/Learned something new:**
Using this and keys to access different variables. Keeps them out of global scope

**Link to work:** 

Hangman commits



### Day 20: January 20th, 2017


**Today's Progress**:
Participated  in a coding Hackathon zoom meeting. Our team created a slack bot.

**Thoughts/Learned something new:**
Saw some different uses of API creation, my first real intro to Node.JS. Got to work with some great people.

**Link to work:** 
Forked 8-ball slack bot


### Day 21: January 21st, 2017


**Today's Progress**: First day of 1st project groups. Reading over Eloquent Javascript and Javascript the good parts, reviewing previous work from Bootcamp. Submitted resume to Anita Smalls (needs work)


**Thoughts/Learned something new:**
var that = this

**Link to work:** 

Just some fiddles today


### Day 22: January 22nd, 2017


**Today's Progress**:


**Thoughts/Learned something new:**


**Link to work:** 




### Day 23: January 23rd, 2017


**Today's Progress**:


**Thoughts/Learned something new:**


**Link to work:** 
