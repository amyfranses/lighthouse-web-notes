# Objects

- Contain **key-value pairs**; each key maps a value
- Contain keys which are always **strings** (or, less commonly, symbols)
- Have unique keys; the same key cannot appear twice in an object
- Have their keys point to values of **any type**

## Object Literals

Values can be represented by literals:

   - string literals - "lighthouse"
   - number literals - 5, 7.5
   - arrays literal syntax - []

   - object literal syntax - {}
   eg 
   ```javascript
   const emptyObject = {};
   const tinyObject = {size: "Tiny"}; 
   ```

### Objects allow us to easily access the values 

eg 
```javascript
const myObject = {
  a: 6,     // Number
  b: "abc", // String
  c: true,  // Boolean
  d: null,  // Null
};
```
To access a value within the object using [] notation
eg
```javascript
const person = { firstName: "Khurram" };
const firstName = person["firstName"]; 
```
NB 
You must put "firstName" in string for otherwisew it will be looking for a variable name that does not exist and will return undefined.

## Assigning a New Value to as Key

```javascript
const mary = { name: "Mary Sue" };
mary["name"] = "Mary Jane";
mary["age"]  = 22;
mary 
```
renamed mary from "Mary Sue" to "Mary Jane"

## Objects as Values

- We can nest objects within objects 
  (key-value pair in an object can have a value that is another object)
eg
```javascript
const person = {
  name: "Paul",
  address: {
    street: "310 W 95th",
    city: "New York",
    zipCode: 10027
  }
};
```
**address** is an object within an object

access city;

```javascript
person["address"]["city"];
```
will output "new york"

## Arrays as Values

```javascript
person["phoneNumbers"] = /* <insert array of phone numbers here> */
```

## Object Keys

- Keys are always strings
- Each key is unique (cannot occur more than once in an object)
- Each key is associated with exactly one value

When writing out object literals the key is always interpreted as a literal string even if unquoted "" .
It is only neccessary to use " " if the key contains spaces, hyphens or periods.

### **Object.keys(...)**

To inspect an object's keys, there is a method Object.keys(...) that returns an array of keys.

# Objects and iteration

JavaScript objects themselves are not iterable in the way the Arrays are.

Instead we need to use a **for...in** statement.

eg
```javascript
var planetMoons = {
  mercury: 0,
  venus: 0,
  earth: 1,
  mars: 2,
  jupiter: 67,
  saturn: 62,
  uranus: 27,
  neptune: 14
};

for (var planet in planetMoons) {
  var numberOfMoons = planetMoons[planet];
  console.log("Planet: " + planet + ", # of Moons: "+ numberOfMoons);
}
```

The variable planet iterates over each key ("mercury", "venus", ...) using the for-loop.

### **There are Limitations of for...in**

