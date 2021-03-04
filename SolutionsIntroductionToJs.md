# Introduction to JavaScript

Solutions are also available [as notebook](https://runkit.com/rikku/introduction-to-javascript---solutions)

## Variables & Datatypes

---

**Exercise 1 a)** Create three variables and assign values with different data types to them

```JavaScript
    // number, string, boolean
    let number = 10
    let name = "Rikku"
    let likesProgramming = true
```

**Exercise 1 b)** Print all the variables using JavaScript's built-in function console.log()

```JavaScript
    console.log(number, name, likesProgramming)
```

**Exercise 1 c)** Print the data type of each variable using JavaScript's built-in keyword "typeof"

```JavaScript
    console.log(typeof number)
```

```JavaScript
    console.log(typeof name)
```

```JavaScript
    console.log(typeof likesProgramming)
```

**Exercise 2** How do we use variables? Explore with arithmetic operators (+, -, \*, /)!

```JavaScript
    // Example
    let firstValue = 3
    let secondValue = 5
```

```JavaScript
    let result = firstValue + secondValue
```

```JavaScript
    result = firstValue - secondValue
```

```JavaScript
    result = firstValue * secondValue
```

```JavaScript
    result = firstValue / secondValue
```

## Arrays

---

<img src="https://i.imgur.com/BkVV97fl.jpg" height=300 />

```JavaScript
    // Example
    let veggies = ['orange', 'lime', 'olive', 'tomato', 'plum', 'maroon']
```

```JavaScript
    veggies[0]
```

```JavaScript
    veggies[1]
```

We can pick one or more from the start, and get a new array of the rest

```JavaScript
    let [firstVeggie, ...otherVeggies] = veggies
```

```JavaScript
    console.log(firstVeggie)
```

We can also create a slice of the array, specifying where to start and end

```JavaScript
    veggies.slice(2, 5)
```

```JavaScript
    veggies.slice(2)
```

```JavaScript
    veggies.slice(0, 2)
```

**Exercise 3 a)** Create an array with names of your friends and print the name of the first, second and then the rest

```JavaScript
    let names = ["Tusse", "Misse", "Nisse", "Lusse"]
```

```JavaScript
    names[0]
```

```JavaScript
    names[1]
```

```JavaScript
    let [,, ...rest] = names
```

```JavaScript
    console.log(rest)
```

**Exercise 3 b)** Log your array of names using different slices

```JavaScript
    names.slice(0,2)
```

```JavaScript
    names.slice(2)
```

```JavaScript
    names.slice(1, 3)
```

**Exercise 4 a)** Count how many names you have added to the a array using array.length

```JavaScript
    names.length
```

**Exercise 4 b)** Change the array, adding a new name first: array = [newItem, ...array]

```JavaScript
    names = ['Hubbe' , ...names]
```

**Exercise 4 c)** Change the array, removing two names: [first, second, ...array] = array

```JavaScript
    [katt1, katt2, ...names] = names
```

Log the removed names. Does it look as expected?

```JavaScript
    console.log(katt1, katt2)
```

**Exercise 4 d)** Remove two names like above, and then ignore them: [, , ...array] = array

```JavaScript
    [, , ...names] = names
```

Log the array. Does it look as expected?

```JavaScript
    console.log(names)
```

**Exercise 4 e)** Combine two arrays of names, using: [...firstArray, ...secondArray]

```JavaScript
    let moreNames = ["Murre", "Miso", "Tasse"]
    names = [...names, ...moreNames]
```

Log the array. Does it look as expected?

```JavaScript
    console.log(names)
```

## For-loops

---

```JavaScript
    // Example
    for (let veggie of veggies) {
        console.log(veggie)
    }
```

```JavaScript
    for (let index in veggies) {
        veggies[index] = veggies[index] + 's'
    }
    console.log(veggies)
```

**Exercise 5 a)** Log each name in your array of names

```JavaScript
    for (let name of names) {
        console.log(name)
    }
```

**Exercise 5 b)** Add a small change to each name in your array

```JavaScript
    for (let index in names) {
        names[index] = names[index] + 's'
    }
    console.log(names)
```

## Objects

---

```JavaScript
    // Example
    let countries = { "sweden" : "stockholm", "great britain" : "london", "japan" : "tokyo" }
```

```JavaScript
    let capital = countries["sweden"]
```

**Exercise 6 a)** Get the capital of Great Britain and Japan using the object "countries"

```JavaScript
    countries["great britain"]
```

```JavaScript
    countries.japan
```

**Exercise 6 b)** Add a new key-value pair to the object "countries"

```JavaScript
    countries.taiwan = 'taipei'
```

**Exercise 6 c)** Update Sweden's capital to Umeå

```JavaScript
    countries.sweden = 'umeå'
```

**Exercise 6 d)** Remove the key-value pair Sweden-Stockholm from the object

```JavaScript
    delete countries.sweden
```

Log the object. Does it look as expected?

```JavaScript
    console.log(countries)
```

**Exercise 6 e)** Print each key-value pair in the object countries

```JavaScript
    for (let [key, value] of Object.entries(countries)) {
        console.log("Country: "+key+", Capital: "+value)
    }
```

## Functions

---

```JavaScript
    // Example
    function myFunction (param1, param2) {
        // Block of code
    }
    (param1, param2) => {
        // Block of code
    }
    // log the name and content
    console.log(myFunction.name)
    console.log(myFunction.toString())
```

```JavaScript
    // arrow functions are anonymous until you assign them to a variable
    let arrowFunction = () => {}
    arrowFunction.name
```

We will start with creating a function that can add two numbers.

```JavaScript
    function addTwoNumbers (number1, number2) {
    let result = number1 + number2
    return result
    }
```

Let's try to use it!

```JavaScript
    addTwoNumbers(1, 2)
```

```JavaScript
    addTwoNumbers(5, 20)
```

**Exercise 7 a)** Create a function that can calculate the difference between two numbers

```JavaScript
    function subtract(number1, number2) {
        let result = number1 - number2
        return result
    }
```

**Exercise 7 b)** Use the function. Does it return the expected results?

```JavaScript
    subtract(5, 20)
```

**Exercise 7 c)** Create a function that can multiply two numbers

```JavaScript
    function multiply(number1, number2) {
        result = number1 * number2
        return result
    }
```

**Exercise 7 d)** Use the function. Does it return the expected results?

```JavaScript
    multiply(5, 20)
```

**Exercise 7 e)** Create a function that can divide two numbers

```JavaScript
    function divide(number1, number2) {
        result = number1 / number2
        return result
    }
```

**Exercise 7 f)** Use the function. Does it return the expected results?

```JavaScript
    divide(5, 20)
```
