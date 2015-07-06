# JavaScript Strings

## Overview

* Concatenation
* Length
* Changing Case
* Replacing Characters
* Turn String to Number
* Splice
* Split
* Resources

## Concatenation

Unlike Ruby, JavaScript doesn't come with a prior knowledge of how to interpolate a variable (remember, interpolation in Ruby looks like this: "#{variable_name}"). 

Instead, when you want to combine several variables into one long string, you must concatenate.

```javascript
var hours = 10;
var species = "sloths";

// the line below prints "sloths sleep 10 hours a day"
console.log(species + " sleep " + hours + " hours a day");
```

## Length

Calling `length` on a string will return the number of characters in that string.

```javascript
var species = "mantis shrimp";

// the line below will print 13
console.log(species.length);
```

## Changing Case

The two common functions to change the case of a string are `toUpperCase()`  and `toLowerCase()`.

```javascript
"I'm not shouting!!!".toUpperCase();
// => "I'M NOT SHOUTING!!!"

"I'M A CONSCIENTIOUS LIBRARIAN.".toLowerCase();
// => "i'm a conscientious librarian."
```
You may notice that there is no pre-built `capitalize()` method. To capitalize just the first letter of a string, you'll have to make your own custom method.

## Replacing Characters

To replace characters with new characters, you can use the `replace()` method. It works similarly to Ruby's `gsub` method in that the first parameter is the set of characters you would like to remove and the second is the string you would like to add instead.

```javascript
"pandas have two compound eyes and a proboscis".replace("pandas", "butterflies");
// => "butterflies have two antennae, two compound eyes, and a proboscis"
```

Notice that the `replace()` will replace only the first occurance:

```javascript
var quote = "xylophone phone home";
quote.replace("o", "*");

// quote is now "xyl*phone phone home"
```

`Replace()` can also take regex for the first parameter:

```javascript
var phoneNumber = "5556768799";

// the line below will return "(555) 676 - 8799"
phoneNumber.replace(/(\d{3})(\d{3})(\d{4})/, '($1) $2 - $3');
```

## Turn String to Number

TODO

## Splice

TODO

## Split

TODO

## Resources

* [StackOverflow - Capitalize the first letter of string](http://stackoverflow.com/a/1026087/2890716)
* [StackOverflow - Replacing all occurrences of a string in JavaScript](http://stackoverflow.com/a/1144788/2890716)
