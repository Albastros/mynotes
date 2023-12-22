# JavaScript String Methods

# JavaScript String Methods

| String length
String slice()
String substring()
String substr()
String replace()
String replaceAll()
String toUpperCase()
String toLowerCase()
String concat() | String trim()
String trimStart()
String trimEnd()
String padStart()
String padEnd()
String charAt()
String charCodeAt()
String split() |
| --- | --- |
|  |  |

# JavaScript String Length

The `length` property returns the length of a string:

# Example

let text = "ABCDEFGHIJKLMNOPQRSTUVWXYZ";

let length = text.length;

# Extracting String Parts

There are 3 methods for extracting a part of a string:

- `slice(*start*, *end*)`
- `substring(*start*, *end*)`
- `substr(*start*, *length*)`

# JavaScript String slice()

`slice()` extracts a part of a string and returns the extracted part in a new string.

The method takes 2 parameters: start position, and end position (end not included).

# Example

Slice out a portion of a string from position 7 to position 13:

let text = "Apple, Banana, Kiwi";let part = text.slice(7, 13);

# JavaScript String substring()

`substring()` is similar to `slice()`.

The difference is that start and end values less than 0 are treated as 0 in `substring()`.

# JavaScript String substr()

`substr()` is similar to `slice()`.

The difference is that the second parameter specifies the **length** of the extracted part.

# Replacing String Content

The `replace()` method replaces a specified value with another value in a string:

# Example

let text = "Please visit Microsoft!";

let newText = text.replace("Microsoft", "W3Schools");

# JavaScript String ReplaceAll()

In 2021, JavaScript introduced the string method `replaceAll()`:

# Example

text = text.replaceAll("Cats","Dogs");text = text.replaceAll("cats","dogs");

# Converting to Upper and Lower Case

A string is converted to upper case with `toUpperCase()`:

A string is converted to lower case with `toLowerCase()`:

---

# JavaScript String toUpperCase()

# Example

let text1 = "Hello World!";

let text2 = text1.toUpperCase();

# JavaScript String toLowerCase()

# Example

let text1 = "Hello World!";       // String

let text2 = text1.toLowerCase();  // text2 is text1 converted to lower

# JavaScript String concat()

`concat()` joins two or more strings:

# Example

let text1 = "Hello";

let text2 = "World";

let text3 = text1.concat(" ", text2);

# JavaScript String trim()

The `trim()` method removes whitespace from both sides of a string:

# Example

let text1 = "      Hello World!      ";

let text2 = text1.trim();

# JavaScript String trimStart()

[ECMAScript 2019](https://www.w3schools.com/js/js_2019.asp) added the String method `trimStart()` to JavaScript.

The `trimStart()` method works like `trim()`, but removes whitespace only from the start of a string.

# Example

let text1 = "     Hello World!     ";

let text2 = text1.trimStart();

# JavaScript String trimEnd()

[ECMAScript 2019](https://www.w3schools.com/js/js_2019.asp) added the string method `trimEnd()` to JavaScript.

The `trimEnd()` method works like `trim()`, but removes whitespace only from the end of a string.

# Example

let text1 = "     Hello World!     ";

let text2 = text1.trimEnd();

# JavaScript String Padding

[ECMAScript 2017](https://www.w3schools.com/js/js_2017.asp) added two new string methods to JavaScript: `padStart()` and `padEnd()` to support padding at the beginning and at the end of a string.

# JavaScript String padStart()

The `padStart()` method pads a string from the start.

It pads a string with another string (multiple times) until it reaches a given length.

# Examples

Pad a string with "0" until it reaches the length 4:

let text = "5";

let padded = text.padStart(4,"0");

Pad a string with "x" until it reaches the length 4:

let text = "5";let padded = text.padStart(4,"x");

# JavaScript String padEnd()

The `padEnd()` method pads a string from the end.

It pads a string with another string (multiple times) until it reaches a given length.

# Examples

let text = "5";

let padded = text.padEnd(4,"0");

let text = "5";let padded = text.padEnd(4,"x");

# Extracting String Characters

There are 3 methods for extracting string characters:

- `charAt(*position*)`
- `charCodeAt(*position*)`
- Property access

---

# JavaScript String charAt()

The `charAt()` method returns the character at a specified index (position) in a string:

# Example

let text = "HELLO WORLD";

let char = text.charAt(0);

---

# JavaScript String charCodeAt()

The `charCodeAt()` method returns the unicode of the character at a specified index in a string:

The method returns a UTF-16 code (an integer between 0 and 65535).

# Example

let text = "HELLO WORLD";

let char = text.charCodeAt(0);

---

# Property Access

ECMAScript 5 (2009) allows property access [ ] on strings:

# Example

let text = "HELLO WORLD";

let char = text[0];