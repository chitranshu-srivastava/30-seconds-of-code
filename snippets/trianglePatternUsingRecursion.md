---
title: triangleUsingRecursion
tags: recursion,pattern,intermediate
firstSeen: 2021-11-21T08:58:16.780Z
---

Print triangle pattern using recursion.

- Function takes an argument, the number of stars in triangle.
- The funtion will reutrn without making a recursive call if the number becomes 1.

```js
const triangleUsingRecursion = (n) => {
  let pattern = "";

  if (n === 1) {
    console.log("*");
    return;
  }

  triangleUsingRecursion(n - 1);

  for (let i = 1; i <= n; i++) {
    pattern += "*";
  }
  console.log(pattern);
};
```

```js
triangleUsingRecursion(5);

/*
Output

*
**
***
****
*****

*/
```
