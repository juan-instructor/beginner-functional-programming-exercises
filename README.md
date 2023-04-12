**IMPORTANT**: To view this document in a human readable format, follow the instructions:

1. Press `ctrl+shift+p` to open the command pallete in Visual Studio Code
2. Type `Markdown preview` and press `enter`

A new pane will open displaying the contents of this markdown.md file in more friendly and human readable format.

<sub>Author:
<a href="https://github.com/Asabeneh/30-Days-Of-JavaScript/blob/master/09_Day_Higher_order_functions/09_day_higher_order_functions.md#returning-function" target="_blank">Asabeneh Yetayeh</a><br>
</sub>

# Functional Programming

We will need a strong foundation in functional programming using Array methods like forEach, map, reduce, filter, find, every, etc.
To get a good grasp of what these methods do, you will need to read/reference the file './array-concepts.md'

**IMPORTANT:** Once you have finished reading about functional programming and array methods in file `array-concepts.md`, provide the solutions to the following problems with their corresponding number in the file `./arrays-solutions.js`

## 💻 Exercises

### Exercises: Level 1

```js
const countries = ["Finland", "Sweden", "Denmark", "Norway", "IceLand"];
const names = ["Asabeneh", "Mathias", "Elias", "Brook"];
const numbers = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10];
const products = [
    { product: "banana", price: 3 },
    { product: "mango", price: 6 },
    { product: "potato", price: " " },
    { product: "avocado", price: 8 },
    { product: "coffee", price: 11 },
    { product: "tea", price: "" },
];
```

1. Explain the difference between **_forEach, map, filter, and reduce_**.
2. Use **_forEach_** to console.log each country in the countries array.
3. Use **_forEach_** to console.log each name in the names array.
4. Use **_forEach_** to console.log each number in the numbers array.
5. Use **_map_** to create a new array by changing each country to uppercase in the countries array.
6. Use **_map_** to create an array of countries length from countries array.
7. Use **_map_** to create a new array by changing each number to its square number (number multiply by itself) in the numbers array
8. Use **_map_** to change to each name to uppercase in the names array
9. Use **_filter_** to filter out countries containing **_land_**. (you can use String.includes() or String.endsWith())
10. Use **_filter_** to filter out countries having six character.
11. Use **_filter_** to filter out countries containing six letters and more in the country array.
12. Use **_filter_** to filter out country start with 'E'; (You can use String.startsWith());
13. Use **_filter_** to filter out only prices with values.
14. Use **_reduce_** to sum all the numbers in the numbers array.
15. Use **_reduce_** to concatenate all the countries and to produce this sentence: **_Estonia, Finland, Sweden, Denmark, Norway, and IceLand are north European countries_**
16. Explain the difference between **_some_** and **_every_**
17. Use **_some_** to check if some names' length greater than seven in names array
18. Use **_every_** to check if all the countries contain the word land
19. Explain the difference between **_find_** and **_findIndex_**.
20. Use **_find_** to find the first country containing only six letters in the countries array
21. Use **_findIndex_** to find the position of the first country containing only six letters in the countries array
22. Use **_findIndex_** to find the position of **_Norway_** if it doesn't exist in the array you will get -1.
23. Use **_findIndex_** to find the position of **_Russia_** if it doesn't exist in the array you will get -1.

### Exercises: Level 2

1. Find the total price of products by chaining these three array iterators(Remember, each Array iterator returns an Array, that is why you can chain)
   (const totalProductsPrice = arr.map(callback).filter(callback).reduce(callback))
2. Find the sum of prices of products using only reduce = reduce(callback)

3. For the following exercises, you need to `import` `countriesList` from `./data/countries-data.js`.

Create a function `countriesInitialLettersCount ` which return an object. This object
holds the letter and the number of times that intial letter occurs in all countryList.
Your output should look like this:

    ```js
    console.log(countriesInitialLettersCount(countryList))
    RETURNS:
    {
      A: 15,
      'Å': 1,
      B: 21,
      U: 8,
      V: 5,
      C: 23,
      D: 4,
      E: 7,
      F: 8,
      G: 16,
      H: 6,
      I: 9,
      J: 4,
      K: 7,
      L: 9,
      M: 23,
      N: 13,
      O: 1,
      P: 12,
      Q: 1,
      R: 5,
      S: 33,
      T: 14,
      W: 2,
      Y: 1,
      Z: 2
    }
    ```

4. Declare a **_getFirstCountries_** function and return an array of countries.
   This function takes two arguments (countryList) and (maximumCountriesInList)

**NOTE**

1. You can ONLY use array.map().filter() in a chain
2. Your output should look like this:

```js
console.log(getFirstCountries(countryList, 2));
// RETURNS:
//[ 'Afghanistan', 'Åland Islands' ]

console.log(getFirstCountries(countryList, 10));
// RETURNS:
[
    "Afghanistan",
    "Åland Islands",
    "Albania",
    "Algeria",
    "American Samoa",
    "Andorra",
    "Angola",
    "Anguilla",
    "Antarctica",
    "Antigua and Barbuda",
];

console.log(getFirstCountries(countryList, 17));
// RETURNS:
[
    "Afghanistan",
    "Åland Islands",
    "Albania",
    "Algeria",
    "American Samoa",
    "Andorra",
    "Angola",
    "Anguilla",
    "Antarctica",
    "Antigua and Barbuda",
    "Argentina",
    "Armenia",
    "Aruba",
    "Australia",
    "Austria",
    "Azerbaijan",
    "Bahamas",
];
```

# Hard Work Pays off - If you need extra practice (specially to get ready for final exam and final projects)

1. Read chapter 4 and 5 on objects and Arrays. Come to my desk whenever you have questions
2. Practice in [freecodecamp](https://www.freecodecamp.org/) - Sign in with your school account
3. Freecodecamp Exercises Arrays
   3.1. [arrays push](https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/basic-javascript/manipulate-arrays-with-push)
   3.2. [arrays pop](https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/basic-javascript/manipulate-arrays-with-pop)
   3.3. [arrays shift](https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/basic-javascript/manipulate-arrays-with-shift)
   3.4. [arrays unshift](https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/basic-javascript/manipulate-arrays-with-unshift)
   3.5 [array exercise 1](https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/basic-javascript/shopping-list)
   3.6 [nested arrays](https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/basic-javascript/accessing-nested-arrays)
   3.8 [array destructuring](https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/es6/use-destructuring-assignment-to-assign-variables-from-arrays)
   3.6. [Review JavaScript Scope](https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/basic-javascript/global-vs--local-scope-in-functions)

4. Objects
   4.1 [Object Lookup](https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/basic-javascript/using-objects-for-lookups)
   4.2. [checking objects for properties](https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/basic-javascript/testing-objects-for-properties)
   4.3 [manipulating comlex objects](https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/basic-javascript/manipulating-complex-objects)
   4.4 [Destructuring](https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/es6/use-destructuring-assignment-to-assign-variables-from-nested-objects)

5. [arrow functions](https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/es6/use-arrow-functions-to-write-concise-anonymous-functions)
   5.1 [default parameters](https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/es6/set-default-parameters-for-your-functions)

6. Modules
   6.1 [Create a module](https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/es6/create-a-module-script)
   6.2 [export](https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/es6/use-export-to-share-a-code-block)
   6.2. [import](https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/es6/reuse-javascript-code-using-import)
   6.3. [default export](https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/es6/import-a-default-export)

7. Finally, expand your knowledge on functional programming
   7.1 [complete freecodecamps section 'functional programming'](https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/functional-programming/learn-about-functional-programming)
