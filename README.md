# Limesharp test

Fork this repo, commit changes after each task and send us the link to your repo (don't do a Pull Request, just send us the link).
We will get back to you shortly. 
Languages accepted: Javascript or PHP. 

### Task 1: 
Make this work (repeat 3 times the contents of an array):
```javascript
repeat([1,2,3]) //[1,2,3,1,2,3,1,2,3]
```
Your solution:

###### if we type in our console your function and repeat([1,2,3]) then the result should be [1,2,3,1,2,3,1,2,3] 

<b>Answer:</b>

```javascript
function repeat(array) {
    let repeatAmount = 3;
    let result = new Array();
    
    for(let i = 0; i < repeatAmount; i++ ) {
        for(let j in array ) {    
           result.push(array[j]);
        }
    }

    return result;
}

repeat([1,2,3]);
```

### Task 2:
Make this work (no vowels, lowercase except the first letter):
```javascript
reformat("liMeSHArp DeveLoper TEST") //Lmshrp dvlpr tst
```
Your solution:

###### if we type in our console your function and reformat("liMeSHArp DeveLoper TEST") then the result should be Lmshrp dvlpr tst

<b>Answer:</b>

```javascript
function reformat(subject) {
    let sub = subject.replace(/[aeiou]/gi, '').toLowerCase();
    return sub.charAt(0).toUpperCase() + sub.slice(1);
}

reformat("liMeSHArp DeveLoper TEST")
```

### Task 3 (optional, for bonus points):
Make this work (without using any built in functions, only a `for` loop, return the next binary number in a string or as an array)
```javascript
next_binary_number([1,0]) // [1,1]

// possible test cases:
// [1,0] => [1,1]
// [1,1] => [1,0,0]
// [1,1,0] => [1,1,1]
// .......
// [1,0,0,0,0,0,0,0,0,1] => [1,0,0,0,0,0,0,0,1,0]
```
Your solution:

###### if we type in our console your function and next_binary_number([1,0,0,0,0,0,0,0,0,1]) then the result should look like 1,0,0,0,0,0,0,0,1,0 (or as an array).

