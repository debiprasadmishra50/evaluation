# Verbal

1. Event loop
2. ES5, ES6 difference and it's operators
3. prototypal Inheritance
4. Why JS does not support multiple constructor
5. What are Promises, Microtask Queue, and states of it
6. Create a program that can execute 3 timeouts synchronously
7. Create a program that uses all concepts of OOPs with real-life examples
8. commonJS and ES module system, show with example
9. What is Server-side and Client-Side rendering
10. Create a Quote Of The Day Application, use this [API Docs](https://quotes.rest) to get Quotes, and print today's quote in a File with proper format
11. Create a function that can flatten any nested the array
    example:

```
    [[1,2,3],4,5,[6,7,[8,9]]] => [1,2,3,4,5,6,7,8,9]
```

11. What are IIFE, give one example
12. Find Output

```js
console.log("[+] START");

setTimeout(() => {
  console.log("Outside timeout 1");
}, 0);

Promise.resolve("Promise resolved 1").then(console.log);

async function run() {
  setTimeout(() => {
    console.log("Inside run Timeout 2");
  }, 0);
}

(() => {
  setTimeout(() => {
    console.log("Inside IIFE Timeout 2");
  }, 0);
})();

run();

Promise.resolve("Promise resolved 2").then(console.log);

console.log("[+] END");
```

# Question

1. Express: Make a MongoDB connetion to the [mongodb+srv://debi:<password>@demo-realm-app.oldhx.mongodb.net/?retryWrites=true&w=majority](mongodb+srv://debi:<password>@demo-realm-app.oldhx.mongodb.net/?retryWrites=true&w=majority) with Password _HZzRaT0O9fDhrIDj_

2. Create a custom middleware to display request time for every request
3. Perform Filteration of data
4. apply rate limiter
5. apply CORS
6. apply JWT auth
7. apply Cross Site Scripting(XSS) Protection

8. Nest
   > 2.1. Setup a NEST application and create a CRUD based on use case(any example will work)
