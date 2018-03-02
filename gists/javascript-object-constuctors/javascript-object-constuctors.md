### JavaScript Object Constructors

try it on [repl.it](https://repl.it/@jasenmichael/JavaScriptObjectConstructors)

```javascript
// Constructor function to create "Person" objects
function Person(first, last, age, eye) {
    this.firstName = first;
    this.lastName = last;
    this.age = age;
    this.eyeColor = eye;
}

// Create a Person object
let someDude = new Person("John", "Doe", 50, "blue")
console.log(someDude)
// add a key value pair to the Person object
someDude.language = "English"
console.log(someDude)


console.log("_______________")


//  Manually create a "Place" object function
function Place(city, state, zip) {
  return {
    city,
    state,
    zip
  }
}

// Create a Place object
let shittyTown = Place('Florence', 'Kentucky', 41042)
console.log(shittyTown)
// add a key value pair to the Place object
shittyTown.isGhetto = true
console.log(shittyTown)


console.log(someDude.firstName + " is from " + shittyTown.city + ", " + shittyTown.state + ".")

```


--------------

##### links:
[Mozilla MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object/constructor)

[W3Schools](https://www.w3schools.com/js/js_object_constructors.asp)
