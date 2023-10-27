# JavaScript Array Method Algorithm
Have you ever wondered how Array methods work under the hood? Do you wish to know what algorithms they use to work their magic? Well I have, and if you're are like me then you have too. So I decided to recreate them to discover what they are actually made of. Please leave a star on this repository if you find this helpful in any way.

<!-- The pop method code section -->
## <code>.pop()</code>
The <strong>pop</strong> method removes the last item of the array and returns that item.

<strong>ALGORITHM</strong>
+ Create a new empty array
+ Loop over current array except the last item
+ Assign the looped over item(s) from the current array to the new array
+ Overwrite the item(s) of the current array with the item(s) of the new array
+ Return the last item of the current array that was added

<br>

```js
let arr = ["Montserrado", "Margibi", "Lofa", "Nimba", "Maryland", "Rivercess", "Gbarpolu", "Bomi", "Sinoe"];

const pop = array => {
  let newArray = [];
  for (let i=0; i<array.length -1; i++){
      newArray[i] = array[i];
  }
  arr = newArray;
  return array[array.length -1];
}

pop(arr);
```

<!-- The push method code section -->
## <code>.push()</code>
The <strong>push</strong> method adds a new item to the end of an array and returns the length of the array.

<strong>ALGORITHM</strong>
+ Check to see if an item was passed or not
+ Add new item to the end of the array
+ Return the length of the array

<br>

```js
let arr = ["Montserrado", "Margibi", "Lofa", "Nimba", "Maryland", "Rivercess", "Gbarpolu", "Bomi", "Sinoe"];

const push = (array, item) => {
  if (item !== undefined) {
    array[array.length] = item;
  }
  return array.length;
} 

push(arr);
```

<!-- The shift method code section -->
## <code>.shift()</code>
The <strong>shift</strong> method removes the first item of the array and returns that item.

<strong>ALGORITHM</strong>
+ Create a new empty array
+ Loop over current array except the first item
+ Assign the looped over item(s) from the current array to the new array
+ Overwrite the item(s) of the current array with the item(s) of the new array
+ Return the first item of the current array that was removed

<br>

```js
let arr = ["Montserrado", "Margibi", "Lofa", "Nimba", "Maryland", "Rivercess", "Gbarpolu", "Bomi", "Sinoe"];

const shift = (array) => {
  let newArray = []; 
  for (let i=1; i<array.length; i++){
    newArray[i -1] = array[i];
  }
  arr = newArray;
  return array[0];
} 

shift(arr);
```

<!-- The unshift method code section -->
## <code>.unshift()</code>
The <strong>unshift</strong> method

```js
let arr = ["Montserrado", "Margibi", "Lofa", "Nimba", "Maryland", "Rivercess", "Gbarpolu", "Bomi", "Sinoe"];




```

<!-- The map method code section -->
## <code>.map()</code>
The <strong>map</strong> method 

```js
let arr = ["Montserrado", "Margibi", "Lofa", "Nimba", "Maryland", "Rivercess", "Gbarpolu", "Bomi", "Sinoe"];




```

<!-- The filter method code section -->
## <code>.filter()</code>
The <strong>filter</strong> method 

```js
let arr = ["Montserrado", "Margibi", "Lofa", "Nimba", "Maryland", "Rivercess", "Gbarpolu", "Bomi", "Sinoe"];




```

<!-- The reduce method code section -->
## <code>.reduce()</code>
The <strong>reduce</strong> method 
```js
let arr = ["Montserrado", "Margibi", "Lofa", "Nimba", "Maryland", "Rivercess", "Gbarpolu", "Bomi", "Sinoe"];




```