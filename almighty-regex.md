# Almighty Regex 

This gist will be describing which types of text in a doccument will match a URL. This will be done using Javascript when implementing the regex.

## Summary
Here is the code for the Regex that will be described in this doccument. 
 /^(https?:\/\/)?([\da-z\.-]+)\.([a-z\.]{2,6})([\/\w \.-]*)*\/?$/
 With this code, any URL will match and be shown in the selections throughout the doccument. It will also show the user if the URL is valid. If it is not a valid URL the regex will not work.

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Grouping Constructs](#grouping-constructs)
- [Bracket Expressions](#bracket-expressions)
- [Character Classes](#character-classes)

## Regex Components
When I first saw the Regex, I was extremely confused and had no clue how to break it down. The goal of this doccument is to describe my research and help the user get a better understanding like I have.
### Anchors
There are two prevelant anchors when using Regex. The first one is ^. This key matches the position before the first character in the string. The $ key has the same concept because it matches the last character in the string. This is done to match how the URL starts and ends.
### Quantifiers
An easy way to indentfy quantifers is to see if the values end with ? or *. In the URL example, we have two of them. The first one checks if the URL has https. This is nexessary for every webpage and is separated by the ?. The other one is separated with * and it has to do with the path of the files. There can be multiple files and they are all checked through this.
### Grouping Constructs
In this Regex, we can break down the components into four parts:
- This is the part which checks if the URL is a https: (https?:\/\/)
- This is the part which checks the path for the webpage: ([\da-z\.-]+)\.
- This is the part which checks whether it has .com, .gov, or any other example that websites all have: ([a-z\.]{2,6})
- This is the part which checks the path where the browser is supposed to send the information the user is looking for: ([\/\w \.-]*)*
### Bracket Expressions
Within the brackets used in this regex, they search for all the letters in lowercase, as well numbers. The brackets are in three out of the four sections in this regex.
### Character Classes
The characters used in the regex are the digits and the alphanumeric characters. \d labels the digets and \w labels the letters.
## Author
This mini tutorial about the regex url was created by Brandon Cruz. 
My github url is: https://github.com/crandonbruz
