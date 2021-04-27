# Part 1a: A Quick Introduction...
## var declaration
1. 20
2. 20
## let declaration
3. 20
4. error, because the variable is only declared and visible inside the if-statement
## const declaration
5. error, because we cannot reassign a const variable after it has been declared
6. error, again because we cannot reassign a const variable after it has been declared
   
# Part 1b: A Little More of a Challenge...
1. It will print out 3 because the length of the prices array is 3 and i is a var declaration which makes it scope the whole function, and accessible outside the for loop.
2. It will print out 150, because in the last iteration of the for loop discountedPrice is set to 300*0.5. And since discountedPrice is a var, it is visible within the scope of the function.
3. It. will print 150, because `Math.round(150 * 100) / 100`, is just 150. And finalPrice is also a var declaration which means it is still visible within the function.
4. returns the array `[50, 100, 150]`, because for each iteration we index each price, multiply it by 0.5 and since all prices were integers finalPrice stayed the same. 
5. It will return an error, because i is a let declaration which means that it is only accessible within the for loop.
6. error, because discountedPrice is also a let declaration making it only available within the for-loop. 
7. It will print 150, because the last iteration of the for loop sets finalPrice to `Math.round(150 * 100) / 100`. And finalPrice is a let declaration with its scope within the function.
8. returns the array `[50, 100, 150]`, because for each iteration we index each price, multiply it by 0.5 and since all prices were integers finalPrice stayed the same. The variable discounted is still valid because it is called within the scope.
9. error, because i is a let declaration and its scope is within the for loop
10. It will print out 3, the length of the array and const is within the scope of the funtion.
11. returns the array `[50, 100, 150]`, since we are still able to push to the const array discounted, and we are not reassigning the const discountedPrice. discounted is within the scope.

## Data Types
12. 
    - A) `student.name`
    - B) `student.['Grad Year']`
    - C) `student.greeting()`
    - D) `student['Favorite Teacher'].name`
    - E) `student.courseLoad[0]`

## Basic Operators & Type Conversion
13. Arithmetic:
    - A) '32', the number 2 gets coverted to a string '2'
    - B) 1, the '3' becomes the number 3 because we are subtracting non-numbers
    - C) 3, null is converted to 0
    - D) '3null', null is converted to 'null' and concatonated to the string '3'
    - E) 4, true is converted to the number 1
    - F) 0, both false and null are converted to the number 0
    - G) '3undefined', undefined is converted to the string 'undefined' and concatonated to '3'
    - H) NaN, undefined is converted to NaN and we are subtracting the number 3 with NaN

14. Comparison:
    - A) True, '2' is converted to its number representation and 2 is greater than 1
    - B) False, the first char '2' is compared with '1'. and '2' is greater than '1'
    - C) True, '2' is converted to the number 2
    - D) False, strict equality compares with type conversion
    - E) False, true is converted to the number 1 which is != to 2
    - F) True, because Boolean(2) is true
15. == is a non-strict regular equality check where operands of different types are converted into numbers and === is for a strict equality check that compares without type conversion.

## Loops
16. look at [code](part1b-question16.js)

## Functions
17. the array `[2, 4, 6]` is returned. In each iteration of the for loop, we loop through each number in the input array and use is as an argument for the doSomething function which doubles the number inputted, then it is appended to the resulting array newArr.

## setInterval(), setTimeout(), clearTimeout()
18. look at [code](part1b-question18.js)
19. it will print:\
    1 \
    4\
    3\
    2