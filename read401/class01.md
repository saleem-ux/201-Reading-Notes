## Review, Research, and Discussion:

## Describe (in plain English) what Array.map() does??
it's a method in javascript that used to iterate over an array and calling function on every element of array and return value. 

## Describe (in plain English) what Array.reduce() does
iterates over an array and returns the last version of the “accumulator” … in each iteration, based on the value and/or idx of the current element in the array, you have the opportunity to modify and return the accumulator. After the last iteration of the array, that accumulator value is returned to the caller.

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
in java script the code run line by line (in order) and if there any function will take time the java script will skip it so for that we use promises we say to java script please finish this function i will wait and then you can go to the other lines.

## Are all callback functions considered to be Asynchronous? Why or Why Not?
taking a callback doesn't make a function asynchronous. There are many examples of functions that take a function argument but are not asynchronous. For example there's forEach in Array. It iterates over each item and calls the function once per item.