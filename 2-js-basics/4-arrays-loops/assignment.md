# Loop an Array

## Instructions

Create a program that lists every 3rd number between 1-20 and prints it to the console.

> TIP: use a for-loop and modify the iteration-expression

## Rubric

| Criteria | Exemplary                               | Adequate                 | Needs Improvement              |
| -------- | --------------------------------------- | ------------------------ | ------------------------------ |
|          | Program runs correctly and is commented | Program is not commented | Program is incomplete or buggy |


testArray = [1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,16,17,18,19,20];

for (let i = 2; i < testArray.length; i = i + 3) {
    console.log(`the next 3rd number is ${testArray[i]}`);
}