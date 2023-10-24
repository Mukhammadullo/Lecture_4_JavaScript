# _1.What is array in JavaScript?_
> _An array is an object that holds values (of any type) not particularly in named properties/keys, but rather in numerically indexed positionIn JavaScript, an array is an ordered list of values. Each value is called an element specified by an index. ... First, an array can hold values of mixed types.An array is a special variable, which can hold more than one value_

```js
let arr=[1,2,"Muhammadullo", [1,2,"Nastulloev"],{name:"Muhammadullo"}]

console.log(arr) //[1,2,"Muhammadullo",[1,2,"Nastulloev"],{name:"Muhammadullo"}]


//change element in array
//1

let arr=[1,2,3,4,5]
arr[0]="Change Element"
console.log(arr) //Change Element

//2

let numbers=[1,2,3,4,5]
numbers[0]="Num1"
numbers[1]="Num2"
numbers[2]="Num3"
numbers[3]="Num4"
numbers[4]="Num5"
console.log(numbers)
//["Num1", "Num2", "Num3", "Num4", "Num5"]

//3
let numbers=[1,2]
arr[2]="Add3"
arr[3]="Add4"
console.log(numbers)
//[1,2,"Add3" , "Add4"]

//4
let numbers=[1,2,3]
numbers[5]="Seven7"
console.log(numbers) //[1,2,3, , ,"Seven7"]
```

# _2.Array Methods_

>> _1.Method-push-The push() method adds one or more elements to the end of an array and returns the new length of the array._
```js
// push

//1
let cars=["BMW", "Opel"]
cars.push("Mercides-Bens")
console.log(cars) // ["BMW", "Opel", "Mercides-Bens"]

//2
let  vegetables=[]
vegetables.push("carrot", "onion", "cucumber")
console.log(vegetables) //["carrot", "onion","cucumber"]

```

>> _2.Method-pop-The pop() method removes the last element from an array and returns that element._
```js
//1
let students=["Hamza", "Amir", "Muhammadullo"]
students.pop()
console.log(students) //["Hamza", "Amir"]

//2
let students=["Hamza", "Amir", "Muhammadullo"]
let last=students.pop()
console.log(last) //Muhammadullo

//3
let students=["Hamza", "Amir", "Muhammadullo"]
let last1=students.pop()
let last2=students.pop()

console.log(students) //["Hamza"]
```
>> _Method-The unshift() method adds one or more elements to the beginning of an array andreturns the new length of the array._

```js
//1
let students=["Amir", "Muhammadullo"]
students.unshift("Hamza")
console.log(students) //["Hamza", "Amir", "Muhammadullo"]

//2
let nums=[]
nums.unshift(1,2)
console.log(nums) //[1,2]
```
>> _Method-The pop() method removes the first element from an array and returns that element._
```js
//pop()

//1
let nums=[1,2,3,4]
nums.shift()
console.log(nums) //[2,3,4]
```

>> _Method splice()-The splice() method takes in two or more arguments. The first argument specifies the starting index from where you want to make changes in the array. The second argument specifies the number of elements you want to remove from the array. If you don't want to remove any elements, you can pass 0 as the second argument._
```js
let fruits = ["apple", "banana", "cherry", "date"];
fruits.splice(1, 2); // Removes 'banana' and 'cherry'
console.log(fruits); // Output: ['apple', 'date']
// Adding elements using splice()
fruits.splice(1, 0, "orange", "grape"); // Inserts 'orange' and 'grape' at index 1
console.log(fruits); // Output: ['apple', 'orange', 'grape', 'date']

// Replacing elements using splice()
fruits.splice(2, 1, "kiwi"); // Replaces 'grape' with 'kiwi' at index 2
console.log(fruits); // Output: ['apple', 'orange', 'kiwi', 'date']

```
>> _Method-indexOf()_
```js
// indexOf() -Array and String method
let students=["Amir", "Hamza", "Muhammadullo"]
let index=students.indexOf("Hamza")
console.log(index) //1
```
>> _Method-includes()_
```js

//includes()- Array and String method

let students=["Hamza", "Amir", "Muhammadullo"]
let newRes=students.includes("Amir") 
console.log(newRes) // true
```
>> _Method-slice()_
```js
//slice ()-Array and Stiring method

let students=["Hamza", "Muhammadullo", "Amir"]
let res=students.slice(1)
console.log(res) //["Muhammadullo", "Amir"]
```

>> _Method concat()_
```js
//concat ()- Array and String method

let students=["Amir"]
let studentsNew=["Muhammadullo", "Hamza"]
let res=students.concat(studentsNew) // ["Amir", "Muhammadullo", "Hamza"]
```

>> _What is JavaScript array methods callbacks-In JavaScript, a callback function is a function that is passed as an argument to another function and is executed inside that function. When it comes to arrays, callback functions are often used with array methods like forEach(), map(), filter(), and reduce()_

>> _forEach() in JavaScript_
```js
let numbers=[1,2,3,4,5]
numbers.forEach(function(element){
    console.log(element*2)
})

//1 ,4, 6, 8,10

```
>> _map()- In JavaScript, the map() method is an array method that creates a new array by calling a callback function on each element of the original array. The callback function is executed for each element, and the returned value is used to populate the new array._

```js
let numbers=[2,3,4]
let newNum=numbers.map(function(element){
    return element*2
})
console.log(newNum) // [2,6,8] 
```

>> _find()In JavaScript, the find() method is an array method that is used to find the first element in an array that satisfies a given condition. It returns the value of the first element that matches the condition, or undefined if no element is found._
```js
let nums=[1,2,3,4]
let res=nums.find(function(element){
    return element > 3
})
console.log(res) //4
```

>> _filter()-The filter() method creates a shallow copy of a portion of a given array, filtered down tojust the elements from the given array that pass the test implemented by the provided function._
```js

```