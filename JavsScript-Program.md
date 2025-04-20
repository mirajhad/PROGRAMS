let arr = "6,3,8,3,5,8,4";

// Convert string to array of numbers, sort them, and join back to a string
let sortedArr = arr
  .split(",")           // ["6", "3", "8", "3", "5", "8", "4"]
  .map(Number)          // [6, 3, 8, 3, 5, 8, 4]
  .sort((a, b) => a - b) // [3, 3, 4, 5, 6, 8, 8]
  .join(",");           // "3,3,4,5,6,8,8"

console.log(sortedArr);
