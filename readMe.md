# Here is the solution

5. 3 timeouts in sync

```js
function wait(secs) {
  return new Promise((resolve, reject) => {
    setTimeout(() => {
      resolve(true);
    }, secs * 1000);
  });
}

async function run() {
  console.log("Start");

  console.log("Waiting 1 secs...");
  await wait(1);

  console.log("1 secs finished");

  console.log("Waiting 2 secs...");
  await wait(2);

  console.log("3 secs finished");

  console.log("Waiting 1 secs...");
  await wait(1);

  console.log("4 secs finished");

  console.log("END");
}

run();
```

10. Flattening Array

```js
const arr = [[1, 2, 3], 4, 5, [6, 7, [8, 9]]];

const res = [];

function flatten(arr) {
  for (let i = 0; i < arr.length; i++) {
    if (typeof arr[i] == "object") {
      flatten(arr[i]);
    } else {
      res.push(arr[i]);
    }
  }

  return res;
}

console.log(flatten(arr));
// flatten(arr);
// console.log(res);
```

12. Freq of each consonant in a string

```js
function test(str) {
  const res = {};

  for (let i = 0; i < str.length; i++) {
    if (
      str[i] === "a" ||
      str[i] === "e" ||
      str[i] === "i" ||
      str[i] === "o" ||
      str[i] === "u" ||
      str[i] === "A" ||
      str[i] === "E" ||
      str[i] === "I" ||
      str[i] === "O" ||
      str[i] === "U"
    )
      continue;
    else res[str[i]] ? res[str[i]]++ : (res[str[i]] = 1);
  }

  return res;
}

console.log(test("abcdefabcdefggghihihihihj"));
```

12. Output

```
[+] START
[+] END
Promise resolved 1
Promise resolved 2
Outside timeout 1
Inside IIFE Timeout 2
Inside run Timeout 2
```
