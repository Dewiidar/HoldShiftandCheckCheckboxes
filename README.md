# 09 - Dev Tools Domination - JavaScript30 Challenge

### Practising:

Console methods

### Notes :

```javascript
// Testing         -important-
const p = document.querySelector("p");

console.assert(p.classList.contains("ouch"), "That is wrong!"); // Display only if the argument is false
```

```javascript
// clearing
console.clear();
```

```javascript
console.log(p); // log the paragraph HTML element without its attributes
console.dir(p); // Shows all the props and methods of the element
```

```javascript
// Grouping together
dogs.forEach(dog => {
  console.groupCollapsed(`${dog.name}`);
  console.log(`This is ${dog.name}`);
  console.log(`${dog.name} is ${dog.age} years old`);
  console.log(`${dog.name} is ${dog.age * 7} dog years old`);
  console.groupEnd(`${dog.name}`);
});
```

```javascript
// counting     -important-
console.count("Wes"); // counts the execution number of firing the console.count() and displays the count number beside the string entered  ex. Wes: 1
console.count("Wes");
```

```javascript
// timing       -important-
console.time("fetching data"); //this is the start of timer
fetch("https://api.github.com/users/dewiidar")
  .then(data => data.json())
  .then(data => {
    console.timeEnd("fetching data"); //this is the start of timer
    console.log(data);
  });
```

```javascript
// table
console.table(dogs);
```

## Getting Started

Clone or download the repository to your local drive.

### Prerequisites

What you need to install:

This project was created using Gulp automation tool, you can run the following command to the local repo directory to install all the dev dependencies

```
npm install
```

### Write gulp in the terminal / command line to run the live server.

## Authors

* **Mohamed Dewidar** - _practising the mentioned methods_ - [Linkedin](https://www.linkedin.com/in/mohamed-dewidar-331252153/)

## License

This project is licensed under the MIT License. (open-source)

## Acknowledgments

* Wesbos - _creator of the challenge_ - (https://github.com/wesbos/JavaScript30)
