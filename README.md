Whiteboarding Friday Project  9/3/2021 Problem #3

Write an algo
Takes a string with repeated characters
Return string that shows how it has been compressed
Will there be spaces or special characters? No spaces, special characters


Input: 'aaaabccdddda'
Output: '3ab2c4da'
Input 'aaa!!!bbbdddggg'
Output: '3a3!3b3d3g'

Pseudocode:
1. Feed stringSquash a string
2. 

function stringSquash(string) {
  let counter = 0;
  let newString = ''
  for(let i = 0; i < string.length; i++) {
    if (string[i] === string[i + 1]) {
      counter++;
    } else if (counter === 0) {
        newString = newString + string[i];
        counter = 0 
        } else {
         newString = newString + (counter + 1) + string[i]
         counter = 0;
         }
     } return newString
     }
 
  }

string = "aaaabccdddda"
newString = '4ab2c4da"


Recursive
1. Base case
2. Termination
3. Recurse

function recursiveSquash(string, i = 0, newString = '') {
  if (i >= string.length) {
    return newString;
    } else if (string[i] === string[i+1]) {
      
      








