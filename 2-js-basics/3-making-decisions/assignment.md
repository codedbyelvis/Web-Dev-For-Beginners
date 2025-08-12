# Operators

## Instructions

Play around with operators. Here's a suggestion for a program you can implement:

You have a set of students from two different grading systems.

### First grading system

One grading system is defined as grades being from 1-5 where 3 and above means you pass the course.

### Second grading system

The other grade system has the following grades `A, A-, B, B-, C, C-` where `A` is the top grade and `C` is the lowest passing grade.

### The task

Given the following array `allStudents` representing all students and their grades, construct a new array `studentsWhoPass` containing all students who pass.

> TIP, use a for-loop and if...else and comparison operators:

```javascript
let allStudents = [
  'A',
  'B-',
  1,
  4,
  5,
  2
]

let studentsWhoPass = [];
```

## Rubric

| Criteria | Exemplary                      | Adequate                      | Needs Improvement               |
| -------- | ------------------------------ | ----------------------------- | ------------------------------- |
|          | Complete solution is presented | Partial solution is presented | Solution with bugs is presented |


const firstGradingSystem = [1,2,3,4,5];
const firstGradingSystemPassing = [3,4,5];
const secondGradingSystem = ['A', 'A-', 'B', 'B-', 'C', 'C-'];
const secondGradingSystemPassing = ['A', 'A-', 'B', 'B-', 'C'];
let allStudents = [
  'A',
  'B-',
  1,
  4,
  5,
  2
]
// array `allStudents` representing all students and their grades


function passesFirstSystem(grade) {
  return firstGradingSystemPassing.includes(grade);
}

const passesSecondSystem = grade =>
secondGradingSystemPassing.includes(grade);

const studentsWhoPass = allStudents.map((grade) => {
  if (typeof grade === 'number') {
      return {
        grade: grade,
        system: 'first',
        hasPassed: passesFirstSystem(grade),
      }; 
  }else if (typeof grade === 'string') {
    return {
      grade: grade,
      system: 'second',
      hasPassed: passesSecondSystem(grade),
    };
  }else {
      console.warn(`Unexpected grade type for: ${grade}`);

      return {
        grade: grade,
        system: 'unknown',
        hasPassed: false,
      };
    }
});
console.log(studentsWhoPass);