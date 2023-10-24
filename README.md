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
let students
```

