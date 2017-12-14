# Introduction


A collection of random number/string generator snippets using `JavaScript`


### random

Basic random number generation using native method

```
console.log(Math.random());
```


### randomInt

Random number within 0 to 100

```
function randomInt(){
	return Math.floor(Math.random()*100);
}

console.log(randomInt());
```


### randomFloat

Random floating point number within 0 to 100

```
function randomFloat(){
	return (Math.random()*100).toFixed(2);
}

console.log(randomFloat());
```
