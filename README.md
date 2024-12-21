# Statistic Calculator HTMl/ CSS/ JS

A Pen created on CodePen.io. Original URL: [https://codepen.io/Mouragheb/pen/WbeoLgN](https://codepen.io/Mouragheb/pen/WbeoLgN).

This project is a Statistics Calculator, implemented using HTML, CSS, and JavaScript. It allows a user to input a list of comma-separated numbers and calculates various statistical metrics, such as mean, median, mode, range, variance, and standard deviation. Here’s a detailed explanation of its components:

1. Structure and Layout (HTML):
	•	HTML elements:
	•	An input form with a text field (<input>), where users can input a list of numbers.
	•	A submit button that triggers a calculation function.
	•	A hidden <div> (id="results") to display calculated results dynamically.
	•	Labels: Explanation for each metric (mean, median, mode, etc.) is provided as <p> tags.

2. Styling (CSS):
	•	The background color is set to #1e6359 (greenish tone) with centered text.
	•	Inputs and buttons have consistent styles to match the aesthetic.
	•	The .hidden class is used to hide the results until the calculation is performed.

3. Functionality (JavaScript):
	•	Helper Functions: Several functions compute statistical metrics:
	•	Mean: Calculates the average of the numbers.
	•	Median: Finds the middle number or the average of the two middle numbers when the list is sorted.
	•	Mode: Determines the most frequently occurring number(s).
	•	Range: Calculates the difference between the largest and smallest number.
	•	Variance: Computes the average squared deviation from the mean.
	•	Standard Deviation: Square root of the variance.
	•	Input Handling:
	•	User input is taken as a comma-separated string and converted into an array of numbers.
	•	Invalid inputs (non-numeric values) are filtered out.
	•	Calculate Function:
	•	Triggers when the user submits the form.
	•	Calls the helper functions to compute metrics.
	•	Displays the results dynamically in the HTML using document.querySelector.

Input and Output Examples:

Example 1:

Input: 2, 4, 6, 8, 10
Explanation:
	•	Mean: Average = (2 + 4 + 6 + 8 + 10) / 5 = 6.
	•	Median: Middle value = 6 (sorted list: 2, 4, 6, 8, 10).
	•	Mode: No number repeats; mode = null.
	•	Range: Max - Min = 10 - 2 = 8.
	•	Variance: Mean = 6, variance = [(2-6)² + (4-6)² + (6-6)² + (8-6)² + (10-6)²] / 5 = 8.
	•	Standard Deviation: √Variance = √8 ≈ 2.83.

Output:
	•	Mean: 6
	•	Median: 6
	•	Mode: null
	•	Range: 8
	•	Variance: 8
	•	Standard Deviation: 2.83

Example 2:

Input: 3, 3, 6, 7, 8, 8, 8
Explanation:
	•	Mean: Average = (3 + 3 + 6 + 7 + 8 + 8 + 8) / 7 ≈ 6.14.
	•	Median: Middle value = 7 (sorted list: 3, 3, 6, 7, 8, 8, 8).
	•	Mode: Most frequent = 8.
	•	Range: Max - Min = 8 - 3 = 5.
	•	Variance: Mean ≈ 6.14, variance ≈ 4.12.
	•	Standard Deviation: √Variance ≈ 2.03.

Output:
	•	Mean: 6.14
	•	Median: 7
	•	Mode: 8
	•	Range: 5
	•	Variance: 4.12
	•	Standard Deviation: 2.03

My Approach:
	1.	The project uses a functional programming style with reusable functions for each metric.
	2.	Dynamic DOM manipulation is used to update the results in real time.
	3.	The design is minimal and user-friendly, focusing on readability and functionality.
	4.	Input validation ensures clean data handling and avoids errors caused by invalid entries.

This project is a great example of combining programming concepts like array manipulation, dynamic updates, and mathematical calculations for a practical use case.
