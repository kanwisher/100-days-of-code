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
See Day 6 folder


### Day 3: January 7th, 2017


**Today's Progress**:

**Thoughts/Learned something new:**

   

**Link to work:** 


### Day 3: January 8th, 2017


**Today's Progress**:

**Thoughts/Learned something new:**

   

**Link to work:** 


### Day 3: January 9th, 2017


**Today's Progress**:

**Thoughts/Learned something new:**

   

**Link to work:** 

### Day 3: January 9th, 2017


**Today's Progress**:

**Thoughts/Learned something new:**

   

**Link to work:** 


### Day 3: January 9th, 2017


**Today's Progress**:

**Thoughts/Learned something new:**

   

**Link to work:** 



### Day 3: January 9th, 2017


**Today's Progress**:

**Thoughts/Learned something new:**

   

**Link to work:** 



### Day 3: January 9th, 2017


**Today's Progress**:

**Thoughts/Learned something new:**

   

**Link to work:** 

