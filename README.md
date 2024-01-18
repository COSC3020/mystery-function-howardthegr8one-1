[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-24ddc0f5d75046c5622901739e7c5dd533143b0c8e959d652212380cedb1ea36.svg)](https://classroom.github.com/a/GDPVb20V)
# Mystery Function

What does the `mystery()` function in the following piece of code do? Add your
answer to this markdown file.

```javascript
function mystery(a) {
    if(a.length == 1) return a[0];
    var foo = mystery(a.slice(1, a.length))
    if(foo > a[0]) return foo;
    else return a[0];
}
```

# My Answer

The mystery function recursively slices the given argument until only a single character/integer is left, and then returns the largest value in the given string/array/etc. 
In the case of a string it will return the highest value number (generally the lower down the alphabet, the 'larger' the character, with uppercase being valued "lower" than lowercase, which has a "higher" value, thus "z" is valued higher than "Z")
