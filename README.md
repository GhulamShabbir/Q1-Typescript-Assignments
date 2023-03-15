# Q1-Typescript-Assignments

Q1 Typescript Assignment
Student: Dr. Ghulam Shabbir

1- Task: Create a Program to Calculate Student Grades
Breakdown:
•	Declare two variables for the exam scores, e.g., englishMarks and urduMarks, and assign them values.
•	Calculate the average of the two exams using the formula: (englishMarks + urduMarks) / 2
•	Use if-else conditionals to determine the student's grade based on the average score.
•	For example, if the average score is greater than or equal to 80, assign grade "A", if it is greater than or equal to 70 and less than 80, assign grade "B", and so on until grade "F" for a score below 60.
•	Display the grade to the user as output.

1- Task: 
Solution 1_ Create a Program to Calculate Student Grades
let englishMarks: number = 85;  
let urduMarks: number = 75;

let average: number = (englishMarks + urduMarks) / 2;

let grade: string;

if (average >= 80) {
  grade = "A";
} else if (average >= 70) {
  grade = "B";
} else if (average >= 60) {
  grade = "C";
} else if (average >= 50) {
  grade = "D";
} else {
  grade = "F";
}
VS Code:
 
Output:
 

Solution 2_ University Grading System
let perc = 45
if (perc >= 90) {
  console.log("A+");
} else if (perc >= 85 && perc < 90) {
  console.log("A");
} else if (perc >= 75 && perc < 85) {
  console.log("B+");
} else if (perc >= 70 && perc < 75) {
  console.log("B");
} else if (perc >= 65 && perc < 70) {
  console.log("C+");
} else if (perc >= 60 && perc < 65) {
  console.log("C");
} else if (perc >= 55 && perc < 60) {
  console.log("D");
} else if (perc < 50) {
  console.log("Fail");

}
console.log(perc);

VS Code:
 
Output:
 



2- Task: Create an Array Manipulation Program
Breakdown:
•	Declare an array of strings, e.g. ["apple", "banana", "cherry", "date", "elderberry"]
•	Use array methods to perform the following manipulations:
o	Append a string to the end of the array
o	Prepend a string to the beginning of the array
o	Remove a string from a specific index in the array and replace it with another string
•	Display the array before and after each manipulation to the user as output.

Typescript Program:
let fruits: string[] = ["apple", "banana", "cherry", "date", "elderberry"];
console.log("Original array: " + fruits);

// Append a string to the end of the array
fruits.push("fig");
console.log("After appending 'fig': " + fruits);

// Prepend a string to the beginning of the array
fruits.unshift("apricot");
console.log("After prepending 'apricot': " + fruits);

// Remove a string from a specific index in the array and replace it with another string
const indexToRemove = 2;
const newFruit = "grape";
fruits.splice(indexToRemove, 1, newFruit);
console.log(`After replacing ${fruits[indexToRemove-1]} with '${newFruit}' at index ${indexToRemove}: ` + fruits);

VS Code:
 
Output:
 

3- Task: Create a Function to Determine the Discount Amount for a Product
Breakdown:
•	Create a function that takes a product price and a discount percentage as input and calculates the discount amount for the product using the formula: discount amount = product price * (discount percentage / 100).
•	If the discount percentage is greater than or equal to 50%, the function should return an error message indicating that the discount percentage is invalid.
•	Display the original price, discount percentage, discount amount, and final price of the product to the user as output.
•	Test the function with different product prices and discount percentages.

Typescript Program:
function calculateDiscount(productPrice: number, discountPercentage: number): number | string {
    if (discountPercentage >= 100) {
      return "Error: Invalid discount percentage.";
    }
    const discountAmount = productPrice * (discountPercentage / 100);
    const finalPrice = productPrice - discountAmount;
    console.log(`Original price: Rs. ${productPrice}`);
    console.log(`Discount percentage: ${discountPercentage}%`);
    console.log(`Discount amount: Rs. ${discountAmount}`);
    console.log(`Final price: Rs. ${finalPrice}`);
    return finalPrice;
  }
  
  // Test the function with different inputs
  calculateDiscount(100, 20);
  calculateDiscount(250, 40);
  calculateDiscount(400, 60);

VS Code:

 
Output:
 

4- Task: Create a Function to Calculate the Factorial of a Number
Breakdown:
•	Create a function that takes a number as input and calculates its factorial using a loop.
•	The factorial of a number is the product of all positive integers less than or equal to the number. For example, the factorial of 5 is 5 x 4 x 3 x 2 x 1 = 120.
•	The function should return the factorial of the input number.
•	Test the function with different numbers to make sure it is working correctly.

Typescript Program:
function calculateFactorial(num: number): number {
  let factorial: number = 1;  // initialize factorial to 1
  
  for (let i = 1; i <= num; i++) {
    factorial *= i;  // multiply factorial by the current number in the loop
  }
  
  return factorial;  // return the final factorial value
}

// Testing the function with different numbers
console.log(calculateFactorial(5));  // output: 120
console.log(calculateFactorial(0));  // output: 1
console.log(calculateFactorial(10)); // output: 3628800


VS Code:
 

Output:
 
