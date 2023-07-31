# javascript

- ## Working with strings

```javascript
let s = "Hello ," + "World"; // Produces Hello , World

/*
 * Obtaining portions of a string
 */

s.substring(1, 5); // "ello": the 2nd, 3re, 4th, and 5th characters
s.slice(1, 5); // "ello": same thing
s.split(","); // ['Hello','World'] : split at delimiter string, it's return a new array
s.split(",", 1); // ['Hello '] : limit number of substring return

/*
 * Searching a string
 */

s.indexOf("W"); // 7 : position of first letter W
s.indexOf("o", 5); // 8 : position of first "o" at or after 5
s.indexOf("oo"); // -1 : does not include the substring "oo"
s.lastIndexOf("l"); // 10 : position of last letter l

/**
 * Boolean searching function in ES6 and later
 */

s.startsWith("ello"); // false : the string does not start these
s.startsWith("Hello"); // true : the string  start with these
s.endsWith("ld"); // true : the string  end with these
s.includes("k"); // false : not includes substring "k"
s.includes("l"); // true : includes substring "k"

/**
 * Creating modified version of a string
 */

s.replace("Hello", "Hi"); // Hi ,world
s.toLowerCase(); // hello ,world
s.toLocaleLowerCase(); // hello ,world
s.toUpperCase(); // HELLO ,WORLD
s.toLocaleUpperCase(); // HELLO ,WORLD
s.normalize(); // Unicode NFC normalization:ES6
s.normalize("NFD"); // NFD normalization ,Also "NFKC","NFKD"

/**
 * Inspecting individual (16-bit) characters of a string
 */

s.charAt(0); // H : the first characters
s.charAt(s.length - 1); // d : the last characters
s.charCodeAt(0); // 72 : 16-bit number at the specified position
s.codePointAt(0); // 72 : ES6, works for codepoints > 16 bits

/**
 * String padding function in ES2017
 */

"A".padStart(3); // "  A" : add spaces on the left to a length of 3
"A".padEnd(3); // "A  " : add spaces on the right to a length of 3
"A".padStart(3, "*"); // "**A" : add star on the left to a length of 3
"A".padEnd(3, "*"); // "A**" : add star on the right to a length of 3

/**
 * Space trimming function trim() is ES5 other ES2019
 */

" test ".trim(); // "test" : remove space on start on end
" test ".trimStart(); // "test" : remove space on start
" test ".trimEnd(); // "test" : remove space on end

/**
 * Miscellaneous string methods
 */

s.concat(" !"); // "Hello ,World !" :  just use + operator instead
"A".repeat(5); // "AAAAA" : concatenate n copies
```

## JavaScript Operators

### Arithmetic Operators

- `+` Addition
- `-` Subtraction
- `*` Multiplication
- `/` Division
- `%` Modulus (Remainder)
- `**` Exponentiation (ES6)

### Assignment Operators

- `=` Assignment
- `+=` Addition assignment
- `-=` Subtraction assignment
- `*=` Multiplication assignment
- `/=` Division assignment
- `%=` Modulus assignment
- `**=` Exponentiation assignment (ES6)
- `<<=` Left shift assignment
- `>>=` Right shift assignment
- `>>>=` Zero-fill right shift assignment
- `&=` Bitwise AND assignment
- `|=` Bitwise OR assignment
- `^=` Bitwise XOR assignment

### Comparison Operators

- `==` Equal to
- `!=` Not equal to
- `===` Equal to and same type
- `!==` Not equal to or not same type
- `>` Greater than
- `<` Less than
- `>=` Greater than or equal to
- `<=` Less than or equal to

### Logical Operators

- `&&` Logical AND
- `||` Logical OR
- `!` Logical NOT

### Bitwise Operators

- `&` Bitwise AND
- `|` Bitwise OR
- `^` Bitwise XOR
- `~` Bitwise NOT
- `<<` Left shift
- `>>` Sign-propagating right shift
- `>>>` Zero-fill right shift

### Conditional (Ternary) Operator

- `condition ? exprIfTrue : exprIfFalse`

### Typeof Operator

- `typeof` Returns a string representing the data type of an operand.

### Instanceof Operator

- `instanceof` Returns true if an object is an instance of a particular constructor.

### Delete Operator

- `delete` Deletes a property from an object or an element from an array.

### Comma Operator

- `,` Evaluates multiple expressions and returns the result of the last expression.

### Void Operator

- `void` Evaluates an expression and returns `undefined`.
