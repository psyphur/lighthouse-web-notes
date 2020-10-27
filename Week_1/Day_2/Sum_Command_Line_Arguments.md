# Sum of Command Line Arguments

## Tips

Break down a problem into smaller helper functions

```javascript
// command line argument getter
const getArguments = () => {
  return process.argv.slice(2);
};

// check whole number
const checkWholeNumber = (value) => {
  const num = Number(value);
  const integer = Number.isInteger(num);

  if (num && integer) {
    return true;
  } else {
    return false;
  }
};

// sum array
const sumArray = (numArray) => {
  let sum = 0;

  for (const value of numArray) {
    let integerNum = Number(value);

    if (checkWholeNumber(integerNum)) {
      sum += integerNum;
    }
  }

  return sum;
}

console.log(sumArray(getArguments()));
```