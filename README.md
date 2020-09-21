# FreeCodeCamp
These are solutions for some of the exercises on FreeCodeCamp

Which freeCodeCamp lessons were most difficult for you and why?

### Introduction to Javascript
**Stand in Line**

-I struggled with this exercise because I did not understand the instructions correctly. I misunderstood the last instruction to “return the element that was removed” and was instead returning the value of nextInLine. I read the first line, function nextInLine(arr, item) {, and automatically assumed that I was supposed to return the value of nextInLine.

When FreeCodeCamp did not accept my first solution, I then change the code to return the value of arr. Since the instructions asked to effect the array via push(), I was returning the new value of arr. When FreeCodeCamp rejected the second solution, I tested my code on the Google console to see what results were being returned. I would see the Google console results and reread the FCC instructions.

Upon rereading the instructions more carefully and reading other people’s comments, I finally understood what the exercise meant by returning the element that was removed from the array. I found two ways to return the element that was removed and stored. The first solution is more concise, and the second solution has an extra step that shows the process more clearly (which is helpful for a beginner coder).

### Introduction to Javascript
**Selecting from Many Options with Switch Statements**

-I followed the format of the sample switch statement when coding the solution to the problem. In the sample switch statement, the value of the cases “a” and “b” were surrounded by quotation marks, so in my solution I quoted the numbers for the cases. I quoted case 1, 2, 3, and 4. Once the solution was rejected, I read a FCC hint: “Remember that case values are tested with strict equality (===).” The cases “a” and “b” in the sample switch statement are quoted because they are strings. The numbers of the cases in the actual exercise do not need to be quoted, because they are not strings but are numbers. I then removed the quotes from the case numbers in my solution.

When writing the code to test each case value, I used “console.log” to print the answer respective to the case value. However, FreeCodeCamp did not accept the solution with the command “console.log”. FCC accepts the commands "return" or "answer = " but not "console.log". This is confusing because when I tested my code with the lines “console.log” on the Google console, it worked fine and it returned the result that FCC was asking for.

### Introduction to Javascript
**Record Collection

-The main difficulty about this exercise is stringing together the lines of code and organizing them in the correct order. I read the rules of the exercise, and then coded in the order that I was reading the rules. For instance, I first read “If prop isn’t tracks” and started coding “if (prop !== tracks).” I attempted to code the instructions in the order that I was reading them.  After getting stuck I realized that it was more efficient to read the entire set of rules a few times and then strategize how to organize my code. Secondly, I oversaw a small mistake that took a bit of time to find. I used the object’s name: “collection” instead of using the word “object” in my code. For example, I coded “delete collection[id][prop];” instead of “delete object[id][prop];.” When FCC did not accept my solution, I reviewed it many times and also tested it on the Google console. I finally realized that I did not rename the property “object” in the array of function updatedRecords. More practice is needed, so that these small mistakes are quicker to catch. 

### Introduction to Javascript
**Profile Lookup** 
-It was difficult to code the solution from scratch. I struggled to recall the appropriate lines of code based on memory. I understood the series of logical steps needed to instruct the computer. The difficult part was remembering the exact codes for specific commands. Once I looked up the solution, I saw that my order of instructions was correct, but the characters were either misplaced or missing. More practice is needed. 

### Introduction to Javascript
**Use Recursion to Create a Range of Numbers**
-I probably struggled the most with the recursion exercises. In this exercise, I am not grasping the order of the numbers. Below is one of the solutions for this exercise:

function rangeOfNumbers(startNum, endNum) {
  if (endNum - startNum === 0) {
    return [startNum];
  } else {
    var numbers = rangeOfNumbers(startNum, endNum - 1);
    numbers.push(endNum);
    return numbers;
  }
}

rangeOfNumbers(1, 5) should return [1, 2, 3, 4, 5]. 

If endNum is 5, it skips the base condition and jumps to the recursive condition. The value of numbers is now [1, 4, 5]. numbers.push(endNum) pushes 5 to the end of the array. Next, 4 - 1 is 3 and numbers is now [1, 4, 3, 5], and so forth until endNum - startNum === 0. I would expect rangeOfNumbers(1, 5) to return [1, 4, 3, 2, 5] but it actually returns [1, 2, 3, 4, 5]. I am struggling to understand the arrangement of the numbers. 

### Introduction to the ES6 Challenges
**Use the Rest Parameter with Function Parameters**

The instructions asked to modify the function sum so that it is able to take any number of arguments and return their sum. When I read “any number of arguments” I thought “number” as a representation of the length of the argument. For example args(2, 3, 4) has 3 arguments, because arg 1, arg 2 and arg 3 sum up to a total of 3 arguments. Therefore, the code I provided used the method “args.length” to return the number or sum of total arguments. The correct answer is to use the method args.reduce instead of args.length. I learned that the method args.reduce is not for subtracting (or adding); it’s used to reduce the number of elements (or arguments for this exercise) and result in one single output. 


### Introduction to the ES6 Challenges
**Create Strings using Template Literals**
The solution for this exercise is:
const failureItems = arr.map(item => `<li class="text-warning">${item}</li>`);

I do not understand the purpose of “item” in the code or what “item” does/represent. I understand the rest of the code. In this lesson’s example, “${person.name}!” and “${person.age}” are also wrapped inside ${ and } like “${item}” in the solution. “person.name” and “person.age” are variables. I do not see how “${item}” is a variable nor what it represents or link back to.





