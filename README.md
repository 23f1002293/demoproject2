# LCM Calculator

## Summary

A minimal, interactive single-page web application to calculate the Least Common Multiple (LCM) of two integers provided by the user.

## Setup

No special setup is required. Follow these steps:

1.  Save the `index.html` file to your local machine.
2.  Open the `index.html` file in any modern web browser (e.g., Chrome, Firefox, Safari).

## Usage

1.  Open the `index.html` file in your browser.
2.  Enter the first number in the "Number 1" input field.
3.  Enter the second number in the "Number 2" input field.
4.  Click the "Calculate LCM" button.
5.  The calculated LCM will be displayed below the button.

## Code Explanation

### `index.html`

The single HTML file contains all the necessary code for the application to run.

-   **HTML Structure**: A basic HTML5 boilerplate with a form. The form includes two `number` inputs for the user, a `submit` button, and a `p` element with the id `result` to display the output.
-   **CSS**: A `<style>` block is included in the `<head>` for minimal styling. It centers the content, provides a clean layout for the form, and styles the inputs and button for a better user experience.
-   **JavaScript**: The core logic is contained within a `<script>` tag at the end of the `<body>`.
    -   **Event Listener**: An event listener is attached to the form's `submit` event to prevent the default page reload and trigger the calculation.
    -   **GCD Function**: A helper function `gcd(a, b)` is implemented using the Euclidean algorithm to find the Greatest Common Divisor of two numbers. This is a crucial step for an efficient LCM calculation.
    -   **LCM Calculation**: The main logic reads the integer values from the input fields. It validates the input and then calculates the LCM using the mathematical formula: `LCM(a, b) = (|a * b|) / GCD(a, b)`. Special handling is included for cases involving zero.
    -   **Display**: The final result or any validation error message is rendered into the `result` paragraph element.

## Version Update Information

**v1.0.0 (2023-10-27)**
-   Initial release.
-   Feature: Calculate and display the LCM of two user-provided numbers.
-   Includes basic input validation and a clean, user-friendly interface.

## License

This project is licensed under the MIT License.
