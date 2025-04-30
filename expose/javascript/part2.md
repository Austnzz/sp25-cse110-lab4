1. Line 12 will end up printing out "3" because i was initialized using the var. that means it is available even outside the for loops
2. It will print out 150 after the arithmetic. it is also accessible outside the for loop as it is initialized using var.
3. This will also print out 150. finalPrice is declared at the top of the function before the for loop and if we compute the followign arithmetic, we also get 150
4. It should return 50, 100, 150. Every one of the price in the input array will get cut by 50% then rounded up.
5. We get an error. This happens because we use let istead of var when declaring i. Becasue let is limited to the for loop code block, the console.log which is outside this scope will see it as undefined.
6. This again will return an error. let discountedPRice is defined inside the for loop. As let is limited to the scope of the block, console.log whcih is outside the loop won't know of its existance.
7. This one will work and output 150. This works out fine since the let finalPrice is declared at the top before the for loop. Thus allowing for console.log to see it.
8. This will return 50, 100, 150. The let declares it at the top so it will exist for when we return it.
9. Similar to before, this will return an error. i was declared using let inside the for loop. this means that console.log outside of it will not be able to see it as it is outside the scope.
10. It will print 3. we declare length as const with the value of prices.length. We don't try to alter this value either and since this is initialized at the top of the function, console.log will be able to access it just fine.
11. This will again return [50,100,150]. if we follow the arithmetic of 1-discount, that is waht we get. then the result is pushed into the array, thus allowing for this to work jsut fine.
12. Given the object above, write the notation for:
- A. student.name
- B. student['Grad Year']
- C. student.greeting()
- D. student['Favorite Teacher'].name
- E. student.courseLoad[0]
13. Arithmetic:
- A. '32' becasue the plus operator triggers concatenation when just one of the inputs is a string so because '3' is a string, it becomes '3' + '2'
- B. 1 because unlike the plus operator, if one of the inputs arent a number it will force both to be making it jsut 3-2=1
- C. 3 because null in a operation like this is just treated as a 0
- D. '3null' because the plus operator sees a string '3' so it trats the null as a string as well and just simply concatenates
- E. 4 because numerically true/false are 1/0 so treating it as such, 3 + 1 = 4 
- F. 0 because false and null are just treated as their numerical values of 0.
- G. '3undefined' because 3 is a string so the plus operator just treats the undefined as one as well, thus simply concatenating both.
- H. NaN because in subtraction, '3' is treated as a number. and 3 - undefined is NaN

14. Comparison:
- A. true because the '2' string is treated as a number
- B. false because both are strings, it uses a lexicographical comparison
- C. true because when using the ==, the '2' string becomes a 2 thus making it equal
- D. false sicne the === checks the value AND the type. So because '2' is a string and 2 is a number, it is false
- E. false because true is treated as a 1 numerically and 1 does not equal 2
- F. true because boolean(2) is true, true === true is true

15. the == sign will only compare the values after doing the necessary conversions. However, === will consider both the value and the type of the inputs. So === tends to be more predicable in terms of what you might want.

16. Find in part2-question16.js

17. The result is 2,4,6. If we look at the modifyArray, it loops through the array 1, 2, 3 then runs the doSomething function on it which doubles the values.

18. Find in part2-question18.js

19. 1
    4
    3
    2
    While console.log(1) and console.lof(4) run pretty much at the same time, we have the setTimeout on 3 and 4 which makes it wait until all the other code has ran. settimeout 0 waits till 1 and 4 runs, then setTimeout 1000 waits a whole second before running.