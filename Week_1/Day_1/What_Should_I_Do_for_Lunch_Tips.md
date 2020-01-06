### Tips

Try experimenting with the comparison operators (`<`, `>`, `===`, etc.) in the node REPL, which you can launch using the `node` command in Vagrant.

Work on your code iteratively – that means in small pieces. 

To help you figure out how to use `hungry` and `availableTime` inside your function, try outputting their values to the Terminal as follows.

```javascript
const whatToDoForLunch = function(hungry, availableTime) {
  let output = "";
  if (hungry === false) {
    // if hungry is false, "wait until you are hungry"
    output = "Wait until you are hungry";
    
    // if hungry is not false, run following code
  } else {
    if (availableTime < 20) {
      output = "Pick something up and eat it back in the lab.";
    } else if (availableTime >= 20 && availableTime <= 30) {
      output = "You deserve a break, try a place in Gastown.";
    } else if (availableTime > 30) {
      output = "This is bootcamp, you don't have more than 30 minutes!";
    }
  }
  console.log(output);
};
```

