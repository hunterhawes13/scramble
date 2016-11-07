## Synopsis

####JavaScript Challenge

Using the JavaScript language, have the function StringScramble(str1,str2) take both parameters being passed and return the string true if a portion of str1 characters can be rearranged to match str2, otherwise return the string false. For example: if str1 is "rkqodlw" and str2 is "world" the output should return true. Punctuation and symbols will not be entered with the parameters. 

## Code Example

```
function StringScramble(str1, str2) { 

  // loop through string 2 
  for (var i = 0; i < str2.length; i++) {
    
    // check if each character also exists in string 1
    // if not, return false
    if (str1.indexOf(str2.charAt(i)) === -1) {
      return false;
    }
    
  }
  
  // return true if all characters exist in string 1
  return true;
         
}
   
StringScramble("rkqodlw", "world");                                                               
```

## Motivation

staying sharp

## Tests
```
Input:"cdore" & str2= "coder"
Output:"true"

Input:"h3llko" & str2 = "hello"
Output:"false"
```

## Contributors

Hunter Hawes
github: hunterhawes13
twitter: @tikishackfun

## License

This project is licensed under the terms of the MIT license.

## Warning

This should not be used in production. It is for demonstration purposes only.
