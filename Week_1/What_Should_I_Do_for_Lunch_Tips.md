# What Should I Do for Lunch Tips

## Tips

Try experimenting with the comparison operators (`<`, `>`, `===`, etc.) in the node REPL, which you can launch using the `node` command in Vagrant.

Work on your code iteratively – that means in small pieces. 

To help you figure out how to use `hungry` and `availableTime` inside your function, try outputting their values to the Terminal as follows.

```javascript 
const whatToDoForLunch = function(hungry, availableTime) {
  if (hungry === true && availableTime < 20) {
    console.log("Pick up something quick and easy and eat in the Lab or Kitchen!");
  } else if (hungry === true && availableTime >= 20 && availableTime < 30) {
    console.log("You deserve a break! Try a restaraunt over at Gastown!");
  } else if (hungry === true && availableTime > 30) {
    console.log("This is a bootcamp program afterall, maybe you should reconsider...");
  } else {
    console.log("Eh... not that hungry anyways, I'll keep going!");
  }
};
```