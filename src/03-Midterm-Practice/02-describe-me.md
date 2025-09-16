# Describe Me - A Lesson on Data Types

![Cute bunch of 4 kittens](./../assets/images/cute-kittens.jpg)

Let's pause for a second and make sure that we understand how data are another way to describe our reality. Different types of data and data structures offer us different ways to carry out this descriptive work.

In small groups of 3-4 people, work through the following sections that ask you to describe the above image of kittens with different types of data primitives and data structures.

<p class="warning">
  Be sure to render your variables to the page in a separate codeblock, so you know the code is working.
</p>

## 1. String

Create a variable that is assigned a String that describes this image in 1-2 sentences.

```js
let cuteKitties = ["This is an image of four cute kittens."]
```

```js
cuteKitties

console.log(cuteKitties)
```

## 2. Array

Create a variable that is assigned to an Array that has 4 or more values to describe this image.

```js
let kittyVibes = ["moody", "orange", "scared", "curious"]
```

```js
kittyVibes

console.log(kittyVibes)
```

## 3. Object

Create a variable that is assigned 1 object with at least 4 key-value pairs.

```js
let kittyFacts = [
  {
    kittyQuantity: 4,
    kittyEyeColor: "blue",
    kittyEyeQuantity: 8,
    kittyAgeMonths: 3
  }
]
```

```js
kittyFacts

console.log(kittyFacts)
```

## 4. Array of Objects

Create a variable that is assigned an Array with 4 objects that represent each kitten. Make sure that each kitten object shares the same keys.

```js
let kittyProfiles = [
  {
    color: "orange",
    position: 2,
    name: "Franklin",
    ageMonths: 3,
  },
  {
    color: "grey-brown stripe",
    position: 1,
    name: "Huey",
    ageMonths: 3,
  },
  {
    color: "grey-brown stripe",
    position: 3,
    name: "Louie",
    ageMonths: 3,
  },
  {
    color: "grey-brown stripe",
    position: 4,
    name: "Dewey",
    ageMonths: 3,
  }
]
```

```js
kittyProfiles

console.log(kittyProfiles)
```

## Helpful Transformative Methods in JS

We should remember a few useful methods, when working with the above types of data. Let's practice some of them together:

### Strings

```js
/**
 * Strings:
 * concatenation, .charAt(), .slice(), .slice()
**/
cuteKitties+" (but they are very naughty)"
```

```js
cuteKitties.charAt(7)
```

### Arrays

```js
/**
 * Arrays:
 * Using index position, .push(), for loops, .map()
**/
kittyVibes.push["mischievous"]

for (let vibe in kittyVibes) {
  console.log("position number:", vibe)
}

let newKittyArray = kittyVibes.map(
  // Accessor function
  (vibe) => {
    if (vibe == "moody") {
      let newVibe = "very "+vibe
      return newVibe
    }
  }
)
```

```js
newKittyArray
```

### Objects

```javascript
/**
 * Objects:
 * Accessing values with keys; Adding new properties (key-value pairs)
**/
```

### Array of Objects

```js
/**
 * Array of Objects:
 * Looping through and accessing properties with keys;
 * Adding new props;
 * Difference between .map() and for loops
**/
let newKittyProfiles = kittyProfiles.map(
  (profile) => {
    if (profile.color == "orange") {
      profile.status = "absolute spaz"
      return profile
    } 
  }
)
```

```js
newKittyProfiles
```