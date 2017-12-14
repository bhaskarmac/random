# Introduction


A collection of possible random number/string generator snippets using `JavaScript`

Following are the different random string/number generation methods using `JavaScript`

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