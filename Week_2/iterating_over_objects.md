# Iterating over Objects

## Tests


// to iterate over an object
```javascript
const object = { a: "1", b: "2", c: "3", d: "4"};
// iterate over object using for in loop
for (const key in object){

  // print ${key} = a, b, c, d
  // print ${object[key]} = values ie 1, 2, 3..

  console.log(`${key}: ${object[key]}`);
  // console.log output will be 
  // a : 1, b : 2, c : 3, d : 4
};

let myArray = Object.keys(object);
  console.log(myArray);
// will print object keys as an array
// eg [a, b, c, d]

  for (const element of myArray){
    console.log(element);
  }
  // will print the value of each element in an array
  ```

**Arrays are objects**
The keys in objects === indexes in arrays

Iterate over an array with the **for in** loop to get the indexes of the array.
