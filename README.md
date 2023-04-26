// A function that checks if a given string is a palindrome
function isPalindrome(str) {
  str = str.toLowerCase().replace(/[^a-z0-9]+/g, ""); // Remove non-alphanumeric characters and convert to lowercase
  return str === str.split("").reverse().join("");
}

// Example usage
console.log(isPalindrome("A man, a plan, a canal, Panama!")); // Output: true
console.log(isPalindrome("Hello, world!")); // Output: false

// A class representing a basic calculator
class Calculator {
  add(a, b) {
    return a + b;
  }
  subtract(a, b) {
    return a - b;
  }
  multiply(a, b) {
    return a * b;
  }
  divide(a, b) {
    if (b === 0) {
      throw new Error("Division by zero!");
    }
    return a / b;
  }
}

// Example usage
const calc = new Calculator();
console.log(calc.add(2, 3)); // Output: 5
console.log(calc.divide(10, 2)); // Output: 5
