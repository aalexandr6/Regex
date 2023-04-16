 Matching an 📧mail Address - Regex Tutorial

Regular Expressions (Regex) is a powerful tool used to search character patterns that resolve a value. We are using the regex below to validate an email address.

``` /^([a-z0-9_.-]+)@([\da-z.-]+).([a-z.]{2,6})$/ ```


## Summary

This Regex is used to make sure the email address that is inputed is valid and has a domain. This tutorial will be going over the components that were used to make up this search pattern. 

## Table of Contents 📖

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Character Classes](#character-classes)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)

### Anchors ⚓️
Assert the current engine postion in string that can match a location. The anchors used in this expression are `^` at the beginning and `$` at the end of the string. It is very useful because that given matching location can be at the begininng of a string or end of a line (subject). They are recomended to use whenever possible. 

### Quantifiers  ✚
``` @([\da-z.-]+). ```

Are used to match up a specific sequence of characters. The quantifier used is `+` to match the username with domains. `+` will make sure to match specified characters or letters to left the of @ to confirm the domain.

### Character Classes  🔤 ➖ 

``` [a-z0-9_.-] ```  ```[a-z.]```

Allows matching characters with the same or different classes. [a-z] is used in begining to accept numbers 0-9 in the email if applicable. It is also used near the end to confirm the ```.``` for (.net) or (.com).

### Grouping and Capturing ```()```
Is being used to group and capture the 3 different types of specified data requirements in the expression for the email with ```()```. ``` ([a-z0-9_.-]+) ``` for username. ``` @([\da-z.-]+) ``` for the domain. ``` .([a-z.]{2,6}) ``` for (.net) or (.com).

### Bracket Expressions ```[]```
They indicate a set of characters to match and can be defined. The information within the brackets in the expression is the sensitive information that we need to match up the email address. 


## Author

This Gist was made by WEB DEV in training AARON P. https://github.com/aalexandr6

Made in partnership with KU BOOTCAMP/EDX
