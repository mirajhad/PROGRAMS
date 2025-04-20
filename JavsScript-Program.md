let arr = "6,3,8,3,5,8,4";
let sortedArr = arr
  .split(",")
  .map(Number)
  .sort((a, b) => a - b)
  .join(",");

console.log(sortedArr);

============================================

const array1 = [5, 2, 8];
const array2 = [3, 9, 1];

const merged = array1.concat(array2);
const sorted = merged.sort((a, b) => a - b);

console.log("Merged and Sorted Array:", sorted);
