# javascript

- ## Working with strings

```javascript
let s = "Hello ," + " World"; // Produces Hello , World

/* Obtaining portions of a string */

s.substring(1, 5); // "ello": the 2nd, 3re, 4th, and 5th characters
s.slice(1, 5); // "ello": same thing
s.split(","); // ['Hello','World'] : split at delimiter string, it's return a new array
s.split(",", 1); // ['Hello '] : limit number of substring return
```
