## Describe (in plain English) what Array.map() does?
it's a method in javascript that used to iterate over an array and calling function on every element of array and return value. 

## Describe (in plain English) what Array.reduce() does
it's a method in javascript that accumulate the values for each element of the array, resulting in a single output value. 

## Provide code snippets showing how to use superagent() to fetch data from a URL and log the result

## With normal Promise .then() syntax
superagent.get("url").then((respone)=>{
    console.log(response.body)
})

## Again with async / await syntax
const asyncFunction = async ()=>{
await superagent.get("url").then((response)=>{
    console.log(response.body)
})
}
asyncFunction();

## Explain promises as though you were mentoring a Code 301 level student
Promises are used to handle asynchronous operations in JavaScript. They are easy to manage when dealing with multiple asynchronous operations
A promise can be created using Promise constructor.
Syntax

>var promise = new Promise(function(resolve, reject){
     //do something
});

## Are all callback functions considered to be Asynchronous? Why or Why Not?
taking a callback doesn't make a function asynchronous. There are many examples of functions that take a function argument but are not asynchronous. For example there's forEach in Array. It iterates over each item and calls the function once per item.