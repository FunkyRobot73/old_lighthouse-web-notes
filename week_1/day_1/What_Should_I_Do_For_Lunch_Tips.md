### Tips

Try experimenting with the comparison operators (`<`, `>`, `===`, etc.) in the node REPL, which you can launch using the `node` command in Vagrant.

Work on your code iteratively – that means in small pieces. 

To help you figure out how to use `hungry` and `availableTime` inside your function, try outputting their values to the Terminal as follows.



```javascript
const whatToDoForLunch = function(hungry, availableTime) {
  if (availableTime < 20 && hungry === true) {
    console.log(`I'm hungry & only have ${availableTime} minutes...  so I'll just eat here.`);
  }
  if (availableTime >= 20 && availableTime <= 30 && hungry === true) {
    console.log(`I'm hungry, ahead & I have ${availableTime} minutes...  I'm going to Gastown.`);
  }
  if (availableTime > 30 && hungry === true) {
    console.log(`I'm hungry & although I have ${availableTime} minutes...  I should get back to coding asap.`);
  }
  if (hungry === false) {
    console.log(`I'm not hungry but even though I have ${availableTime} minutes... I'll continue to work.`);
  }

};


/*
 * This is some test runner code that's simply calling our whatToDoForLunch function
 * defined above to verify we're making the right decisions. Do not modify it!
 */

console.log(".");
whatToDoForLunch(true, 20);
console.log("---");

console.log(".");
whatToDoForLunch(true, 50);
console.log("---");

console.log(".");
whatToDoForLunch(false, 30);
console.log("---");

console.log(".");
whatToDoForLunch(true, 15);
```