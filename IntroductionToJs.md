# Introduction to JavaScript

Recommended way to solve the exercises:
[Clone this Notebook](https://runkit.com/rikku/introduction-to-javascript)

Alternatively, use a console in your browser Developer Tools (it will be harder to save your progress).

## Variables & Datatypes

---

**Exercise 1 a)** Create three variables and assign values with different data types to them

```JavaScript
    // number, string, boolean

```

**Exercise 1 b)** Print all the variables using JavaScript's built-in function console.log()

```JavaScript

```

**Exercise 1 c)** Print the data type of each variable using JavaScript's built-in keyword "typeof"

```JavaScript

```

```JavaScript

```

```JavaScript

```

**Exercise 2** How do we use variables? Explore with arithmetic operators (+, -, \*, /)!

```JavaScript
    // Example
    let firstValue = 3
    let secondValue = 5

    let result = firstValue + secondValue
    console.log(result)
```

```JavaScript

```

```JavaScript

```

```JavaScript

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

```

```JavaScript

```

```JavaScript

```

```JavaScript

```

**Exercise 3 b)** Log your array of names using different slices

```JavaScript

```

```JavaScript

```

```JavaScript

```

**Exercise 4 a)** Count how many names you have added to the a array using array.length

```JavaScript

```

**Exercise 4 b)** Change the array, adding a new name first: array = [newItem, ...array]

```JavaScript

```

**Exercise 4 c)** Change the array, removing two names: [first, second, ...array] = array

```JavaScript

```

Log the removed names. Does it look as expected?

```JavaScript

```

**Exercise 4 d)** Remove two names like above, and then ignore them: [, , ...array] = array

```JavaScript

```

Log the array. Does it look as expected?

```JavaScript

```

**Exercise 4 e)** Combine two arrays of names, using: [...firstArray, ...secondArray]

```JavaScript

```

Log the array. Does it look as expected?

```JavaScript

```

## For-loops

---

```JavaScript
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

```

**Exercise 5 b)** Add a small change to each name in your array

```JavaScript

```

## Objects

---

```JavaScript
    // Example
    let countries = { "sweden" : "stockholm", "great britain" : "london", "japan" : "tokyo" }
```

```JavaScript
    let capital = countries["sweden"]
    console.log(capital)
```

**Exercise 6 a)** Get the capital of Great Britain and Japan using the object "countries"

```JavaScript

```

**Exercise 6 b)** Add a new key-value pair to the object "countries"

```JavaScript

```

**Exercise 6 c)** Log the object. Does it look as expected?

```JavaScript

```

**Exercise 6 d)** Update Sweden's capital to Umeå

```JavaScript

```

**Exercise 6 e)** Log the object. Does it look as expected?

```JavaScript

```

**Exercise 6 f)** Remove the key-value pair Sweden-Stockholm from the object

```JavaScript

```

**Exercise 6 g)** Log the object. Does it look as expected?

```JavaScript

```

**Exercise 6 h)** Print each key-value pair in the object countries

```JavaScript

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

```

**Exercise 7 b)** Use the function. Does it return the expected results?

```JavaScript

```

**Exercise 7 c)** Create a function that can multiply two numbers

```JavaScript

```

**Exercise 7 d)** Use the function. Does it return the expected results?

```JavaScript

```

**Exercise 7 e)** Create a function that can divide two numbers

```JavaScript

```

**Exercise 7 f)** Use the function. Does it return the expected results?

```JavaScript

```
