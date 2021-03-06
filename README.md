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

### randomString

Random string

```
function randomString() {
  var text = "";
  var charSet = "ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz";

  for (var i = 0; i < 6; i++)
    text += charSet.charAt(Math.floor(Math.random() * charSet.length));

  return text;
}

console.log(randomString());
```

### randomAlphaNumString

Random alpha numeric string

```
function randomAlphaNumString(len) {
  var text = "";
  var charSet = "0123456789ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz";

  for (var i = 0; i < len; i++)
    text += charSet.charAt(Math.floor(Math.random() * charSet.length));

  return text;
}

console.log(randomAlphaNumString());
```

### randomArrMember

Random member of given Array

```
function randomArrMember(arr) {
if(arr.length){
  for (var i = 0; i < arr.length; i++)
    return arr[Math.floor(Math.random() * arr.length)];
   } else{
    return;
   }
}

console.log(randomArrMember());
```