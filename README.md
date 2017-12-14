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

Random floating point number within 0 to 100 with 2 decimal points

```
function randomFloat(){
	return (Math.random()*100).toFixed(2);
}

console.log(randomFloat());
```


### randomIntInRange

Random number within `min` and `max`

```
function randomIntInRange(min, max){
	return Math.random() * (max - min) + min;
}

console.log(randomIntInRange(1, 1000));
```


### randomFloatInRange

Random floating point number within `min` and `max` with 2 decimal points

```
function randomFloatInRange(min, max){
	return (Math.random() * (max - min) + min).toFixed(2);
}

console.log(randomFloatInRange(1, 1000));
```


### randomHex

Random hex value

```
function randomHex(){
	return '#'+Math.floor(Math.random()*16777215).toString(16);
}

console.log(randomHex());
```