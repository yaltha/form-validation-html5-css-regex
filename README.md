# form-validation-html5-css-regex
Form input validation with css and regular expression in html5.

Based on the project [here](https://codepen.io/helgesverre/pen/vWRevp)
Also I reference this [Ideas by Frorin Pop github](https://github.com/florinpop17/app-ideas/blob/master/Projects/1-Beginner/Javascript-Validation-With-Regex.md)

Key Points in this project:
1. HTML5:
  - using 'pattern' atribute in the input, that is matching pattern of the regex
  - using 'data-validation-text' in the span to reference the this atribute to css selector
3. Regex
  - pattern=".{5,}" => to match for minimum 5 chars to be typed.
  - pattern="[a-z0-9._%+-]+@[a-z0-9.-]+\.[a-z]{2,63}$" => for valid patern.
  - pattern="([0-9]|\s){2,}"  => for phone number pattern
5. CSS  
  - input:invalid:not(:placeholder-shown)  => when the inout is invalid and not blank
  - input:invalid:not(:placeholder-shown) + [data-validation-text]  => when input is invalid , show and make the adjacent validation text red
