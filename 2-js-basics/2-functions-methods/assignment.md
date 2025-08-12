# Fun with Functions

## Instructions

Create different functions, both functions that return something and functions that don't return anything.

See if you can create a function that has a mix of parameters and parameters with default values.

## Rubric

| Criteria | Exemplary                                                                              | Adequate                                                         | Needs Improvement |
| -------- | -------------------------------------------------------------------------------------- | ---------------------------------------------------------------- | ----------------- |
|          | Solution is offered with two or more well-performing functions with diverse parameters | Working solution is offered with one function and few parameters | Solution has bugs |

1. const noReturn = (emotion) => {
    console.log(`I do not return. This makes me feel ${emotion}`);
}
2. function iReturn(count, emotion) {

    for(let i=0; i < count; i++) {}    
    
    return `I have returned ${count} times, and that makes me ${emotion}!`
}
console.log(iReturn(4, "happy"));