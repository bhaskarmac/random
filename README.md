# Introduction


A collection of possible random number/string generator snippets using `JavaScript`


### random

Basic random number generation using native method


```
console.log(Math.random());

//generates like numbers 0.49561054427985707
```


### randomInt

Random number within 0 to 100

```
function randomInt(){
	return Math.floor(Math.random()*100);
}

console.log(randomInt());

//generates random number within 0 to 100
```


### randomFloat

Random floating point number within 0 to 100

```
function randomFloat(){
	return (Math.random()*100).toFixed(2);
}

console.log(randomFloat());

//generates random floating point number within 0 to 100
```
