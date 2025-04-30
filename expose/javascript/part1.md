1. 
The value 20 is printed out. Because we pass the "add" variable as true, once it passes the id statement, we do result = num1 + num2 which results inresult being added together.

2. 
Line 13 also prints out 20. Likewise, because the add is passed as true, it runs the if statement leading to the result being num1 + num2. But because it is outside the if statment it waits for that to be ran before printing.

3. 
var is accessible anywhere in the function even inside of blocks. These declaration end up being moved to the top of the function, meaning even if you declare or use anew variable alter on, JS moves it to the top when compiled

4. 
This should again print 20. Solong as add is true and we continue doing the same arithmetic, this will always be 10 + 10

5. 
This time this should raise an error. This si because instead of using var to declare the variable, we use let. This makes it so the changes and the declaration of the variable remains inside the if block. So, when we do console.log, result doesnt exist for it.

6. 
This will likely be an error. Because we are assigning result to be a constant, we can't reassign its value. So the arithmetic of num1 +num2 won't work

7. 
This will also throw an error, since like number 5, the reference isn't defined in its scope. Because it is a const, it is limited to only the if block it was declared in