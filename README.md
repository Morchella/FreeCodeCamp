# FreeCodeCamp
These are solutions for some of the exercises on FreeCodeCamp

Basic JavaScript: Stand in Line
I misunderstood the last instruction to “return the element that was removed.” I was instead coding to return the value of nextInLine. I looked at the first line of code, function nextInLine(arr, item) {, and automatically assumed that I was supposed to call for the value of nextInLine. 

When FreeCodeCamp did not accept my first solution, I then called to return the value of arr. Since the instructions asked to change the array by pushing and adding a number to the end of the array, and then removing the first element of the array, my brain went on autopilot and assumed that FCC must want the new value of arr. When FreeCodeCamp rejected the second solution, I tested my code on the Google console to see what information it was returning. I would see the Google console results and reread the FCC instructions to see the results they were asking for. 

Upon rereading the instructions more carefully and googling other people’s comments, I finally understood what the exercise meant by returning the element that was removed from the array. I found two ways to return the element that was removed and stored. The first solution is more concise, and the second solution has an extra step that shows the process more clearly (which is helpful for a beginner coder). 

Short answer:

function nextInLine(arr, item) {
  arr.push(item);
  return arr.shift();
}

Alternate answer:

function nextInLine(arr, item) {
  arr.push(item);
  var removed = arr.shift();
  return removed; 
}
-----------------------------

Basic JavaScript: Selecting from Many Options with Switch Statements

I followed the format of the sample switch statement when coding the solution to the problem. In the sample switch statement, the value of the cases “a” and “b” were surrounded by quotation marks, so in my solution I quoted the numbers for the cases. I quoted case 1, 2, 3, and 4. Once the solution was rejected, I read a hint to the answer: “Remember that case values are tested with strict equality (===).” The cases “a” and “b” in the sample switch statement are quoted because they are strings. The numbers of the cases in the actual exercise do not need to be quoted, because they are not strings but values that strictly equal to their respective numbers. I then removed the quotes from the case numbers in my solution. 

When writing the code to test each case value, I wrote “console.log” to print the answer respective to the case value.  However, FreeCodeCamp did not accept the solution with the line of code “console.log”. FCC accepts the commands “return” or “answer = “ instead of “console.log”. This is confusing because when I tested my code with the lines “console.log” on the Google console, it worked fine and it returned the result that FCC was asking for. I, therefore, replaced “console.log(“”)” with return “” and the code was accepted by FCC.

Second Solution: 

function caseInSwitch(val) {
  var answer = "";
  switch(val) {
    case 1:
      console.log("alpha")
      break;
    case 2:
      console.log("beta");
      break;
    case 3:
      console.log("gamma");
      break;
    case 4:
      console.log("delta");
      break;  
  }
}

caseInSwitch(1);

Third (Submitted) Solution: 

function caseInSwitch(val) {
  var answer = "";
  switch(val) {
    case 1:
      return "alpha";
      break;
    case 2:
      return "beta";
      break;
    case 3:
      return "gamma";
      break;
    case 4:
      return "delta";
      break;  
  }
}

