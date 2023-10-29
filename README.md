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

<br>

<strong>RESULT</strong>
```js
"Sinoe"
```

<br>

<!-- The push method code section -->
## <code>.push()</code>
The <strong>push</strong> method adds a new item to the end of an array and returns the new length of the array.

<strong>ALGORITHM</strong>
+ Check to see if an item was passed or not
+ Add the new item to the end of the array
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

push(arr, "Grand Kru");
```

<br>

<strong>RESULT</strong>
```js
10
```

<br>

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

<br>

<strong>RESULT</strong>
```js
"Montserrado"
```

<br>

<!-- The unshift method code section -->
## <code>.unshift()</code>
The <strong>unshift</strong> method adds an item to the beginning of the array and returns the new length of the array.

<strong>ALGORITHM</strong>
+ Check to see if an item was passed or not
+ Create a new array and assign the new item to it
+ Loop over the current array and add the items to the new array
+ Overwrite the current array with the new array
+ Return the new length of the current array

<br>

```js
let arr = ["Montserrado", "Margibi", "Lofa", "Nimba", "Maryland", "Rivercess", "Gbarpolu", "Bomi", "Sinoe"];

const unshift = (array, item) => {
  if (item !== undefined){
    let newArray = [item];
    for (let i=0; i<array.length; i++){
      newArray[i+1] = array[i];
    }
    arr = newArray;
  }
  return arr.length;
}

unshift(arr, "Grand Kru");
```

<br>

<strong>RESULT</strong>
```js
10
```

<br>

<!-- The map method code section -->
## <code>.map()</code>
The <strong>map</strong> method runs a function on each item of the current array and returns the result in a new array.

<strong>ALGORITHM</strong>
+ Create a new array
+ Loop over the current array
+ Run an IIFE on each item of the current array and add the return value to the new array
+ Return the new array

<br>

```js
let arr = ["Montserrado", "Margibi", "Lofa", "Nimba", "Maryland", "Rivercess", "Gbarpolu", "Bomi", "Sinoe"];

const map = array => {
  let newArray = [];
  for (let i=0; i<array.length; i++){
    newArray[i] = function() {
      return array[i] + " County";
    }();
  }
  return newArray;
}

map(arr);
```

<br>

<strong>RESULT</strong>
```js
['Montserrado County', 'Margibi County', 'Lofa County', 'Nimba County', 'Maryland County', 'Rivercess County', 'Gbarpolu County', 'Bomi County', 'Sinoe County']
```

<br>

<!-- The filter method code section -->
## <code>.filter()</code>
The <strong>filter</strong> method 

<br>

```js
let arr = ["Montserrado", "Margibi", "Lofa", "Nimba", "Maryland", "Rivercess", "Gbarpolu", "Bomi", "Sinoe"];




```

<br>

<strong>RESULT</strong>
```js
```

<br>

<!-- The reduce method code section -->
## <code>.reduce()</code>
The <strong>reduce</strong> method 

<br>

```js
let arr = ["Montserrado", "Margibi", "Lofa", "Nimba", "Maryland", "Rivercess", "Gbarpolu", "Bomi", "Sinoe"];




```

<br>

<strong>RESULT</strong>
```js
```

<br>

<!-- The reduceRight method code section -->
## <code>.reduceRight()</code>
The <strong>reduceRight</strong> method 

<br>

```js
let arr = ["Montserrado", "Margibi", "Lofa", "Nimba", "Maryland", "Rivercess", "Gbarpolu", "Bomi", "Sinoe"];




```

<br>

<strong>RESULT</strong>
```js
```

<br>

<!-- The slice method code section -->
## <code>.slice()</code>
The <strong>slice</strong> method 

<br>

```js
let arr = ["Montserrado", "Margibi", "Lofa", "Nimba", "Maryland", "Rivercess", "Gbarpolu", "Bomi", "Sinoe"];




```

<br>

<strong>RESULT</strong>
```js
```

<br>

<!-- The splice method code section -->
## <code>.splice()</code>
The <strong>splice</strong> method 

<br>

```js
let arr = ["Montserrado", "Margibi", "Lofa", "Nimba", "Maryland", "Rivercess", "Gbarpolu", "Bomi", "Sinoe"];




```

<br>

<strong>RESULT</strong>
```js
```

<br>

<!-- The forEach method code section -->
## <code>.forEach()</code>
The <strong>forEach</strong> method 

<br>

```js
let arr = ["Montserrado", "Margibi", "Lofa", "Nimba", "Maryland", "Rivercess", "Gbarpolu", "Bomi", "Sinoe"];




```

<br>

<strong>RESULT</strong>
```js
```

<br>

<!-- The includes method code section -->
## <code>.includes()</code>
The <strong>includes</strong> method 

<br>

```js
let arr = ["Montserrado", "Margibi", "Lofa", "Nimba", "Maryland", "Rivercess", "Gbarpolu", "Bomi", "Sinoe"];




```

<br>

<strong>RESULT</strong>
```js
```

<br>

<!-- The find method code section -->
## <code>.find()</code>
The <strong>find</strong> method 

<br>

```js
let arr = ["Montserrado", "Margibi", "Lofa", "Nimba", "Maryland", "Rivercess", "Gbarpolu", "Bomi", "Sinoe"];




```

<br>

<strong>RESULT</strong>
```js
```

<br>

<!-- The some method code section -->
## <code>.some()</code>
The <strong>some</strong> method 

<br>

```js
let arr = ["Montserrado", "Margibi", "Lofa", "Nimba", "Maryland", "Rivercess", "Gbarpolu", "Bomi", "Sinoe"];




```

<br>

<strong>RESULT</strong>
```js
```

<br>

<!-- The every method code section -->
## <code>.every()</code>
The <strong>every</strong> method 

<br>

```js
let arr = ["Montserrado", "Margibi", "Lofa", "Nimba", "Maryland", "Rivercess", "Gbarpolu", "Bomi", "Sinoe"];




```

<br>

<strong>RESULT</strong>
```js
```

<br>

<!-- The sort method code section -->
## <code>.sort()</code>
The <strong>sort</strong> method 

<br>

```js
let arr = ["Montserrado", "Margibi", "Lofa", "Nimba", "Maryland", "Rivercess", "Gbarpolu", "Bomi", "Sinoe"];




```

<br>

<strong>RESULT</strong>
```js
```

<br>

<!-- The reverse method code section -->
## <code>.reverse()</code>
The <strong>reverse</strong> method 

<br>

```js
let arr = ["Montserrado", "Margibi", "Lofa", "Nimba", "Maryland", "Rivercess", "Gbarpolu", "Bomi", "Sinoe"];




```

<br>

<strong>RESULT</strong>
```js
```

<br>

<!-- The findIndex method code section -->
## <code>.findIndex()</code>
The <strong>findIndex</strong> method 

<br>

```js
let arr = ["Montserrado", "Margibi", "Lofa", "Nimba", "Maryland", "Rivercess", "Gbarpolu", "Bomi", "Sinoe"];




```

<br>

<strong>RESULT</strong>
```js
```

<br>

<!-- The indexOf method code section -->
## <code>.indexOf()</code>
The <strong>indexOf</strong> method 

<br>

```js
let arr = ["Montserrado", "Margibi", "Lofa", "Nimba", "Maryland", "Rivercess", "Gbarpolu", "Bomi", "Sinoe"];




```

<br>

<strong>RESULT</strong>
```js
```

<br>

<!-- The lastIndexOf method code section -->
## <code>.lastIndexOf()</code>
The <strong>lastindexOf</strong> method 

<br>

```js
let arr = ["Montserrado", "Margibi", "Lofa", "Nimba", "Maryland", "Rivercess", "Gbarpolu", "Bomi", "Sinoe"];




```

<br>

<strong>RESULT</strong>
```js
```

<br>

<!-- The concat method code section -->
## <code>.concat()</code>
The <strong>concat</strong> method 

<br>

```js
let arr = ["Montserrado", "Margibi", "Lofa", "Nimba", "Maryland", "Rivercess", "Gbarpolu", "Bomi", "Sinoe"];




```

<br>

<strong>RESULT</strong>
```js
```

<br>

<!-- The join method code section -->
## <code>.join()</code>
The <strong>join</strong> method 

<br>

```js
let arr = ["Montserrado", "Margibi", "Lofa", "Nimba", "Maryland", "Rivercess", "Gbarpolu", "Bomi", "Sinoe"];




```

<br>

<strong>RESULT</strong>
```js
```

<br>