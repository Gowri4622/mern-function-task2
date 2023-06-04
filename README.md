### EX NO: 09

# <p align="center">Finding ancestor and offspring</P>

## Aim:
The aim of the given code is to create a function that takes a number and a character representing the gender ("m" for male, "f" for female) and 
returns the name of an ancestor (m/f) or descendant (m/f) based on the input values.

## Algorithm:

Step 1: Create a function named check that takes two parameters: num (the 
number representing the generation) and gen (the character 
representing the gender).

Step 2: Inside the function, check the value of gen to determine whether it 
represents a male or female.

Step 3: If gen is equal to 'f', execute the following steps:
• Use a switch statement to check the value of num<br>
• If num is -1, print "Mother".<br>
• If num is -2, print "Grand Mother".<br>
• If num is -3, print "Great Grand Mother".<br>
• If num is 0, print "ME".<br>
• If num is 1, print "Daughter".<br>
• If num is 2, print "Grand Daughter".<br>
• If num is 3, print "Great Grand Daughter".

Step 4: If gen is equal to 'm', execute the following steps:
• Use a switch statement to check the value of num<br>
• If num is -1, print "Father".<br>
• If num is -2, print "Grand Father".<br>
• If num is -3, print "Great Grand Father".<br>
• If num is 0, print "ME".<br>
• If num is 1, print "Son".<br>
• If num is 2, print "Grand Son".<br>
• If num is 3, print "Great Grand Son".<br>

Step 5: Close the switch statement and the if-else statement.
  
Step 6: Call the check function with the arguments 1 and 'f'.
  



## Program

### script.js
```
function check(num,gen)
{
 if(gen=='f')
 {
 switch(num)
 {
 case -1:
 console.log("Mother")
 break
 case -2:
 console.log("Grand Mother")
 break
 case -3:
 console.log("Great Grand Mother")
 break
 case 0:
 console.log("ME")
 break
 
 case 1:
 console.log("Daughter")
 break
 case 2:
 console.log("Grand Daughter")
 break
 
 case 3:
 console.log("Great Grand Daughter")
 break
 }
 }
 else if(gen == 'm')
 {
 switch(num)
 {
 case -1:
 console.log("Father")
 break
 case -2:
 console.log("Grand Father")
 break
 case -3:
 console.log("Great Grand Father")
 break
 case 0:
 console.log("ME")
 break
 
 case 1:
 console.log("Son")
 break
 case 2:
 console.log("Grand Son")
 break
 
 case 3:
 console.log("Great Grand Son")
 break
}
}
}
check.call(this,1,'f')
```

## Output
![image](https://github.com/Gowri4622/mern-function-task2/assets/75235455/06277865-46a0-496c-8c3b-fee9060fca4e)


## Result
The output of the given code, when calling the check function with 1 as num and 'f' as gen, will be "Daughter".

