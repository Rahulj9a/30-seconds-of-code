---
title: Create random letter
tags: math, random, array
expertise: beginner
firstSeen: 2022-07-03T15:40:39+05:30
---

Generate a random letter lowercase or uppercase

- Use `Math.random()` to generate a random value, map it to the desired range using multiplication.
- Use `Math.floor()` to make it an integer
- Use `Array[index]` to pickup a letter from the array  

```js
 const lowerCaseLetters = ["a", "b", "c", "d", "e", "f", "g", "h", "i", "j", "k", "l", "m", "n", "o", "p", "q", "r", "s", "t", "u", "v", "w", "x", "y", "z"];
 const randomLetter = (caseType) =>
        (caseType === "upper" || caseType === "Upper") ?
            lowerCaseLetters[Math.floor(Math.random() * 26)].toUpperCase()
            :
            lowerCaseLetters[Math.floor(Math.random() * 26)]

```

```js
 randomLetter('upper'); // 'W'
```
