# console-to-page
An HTML file that redirects the Developer Tools console output to the page. It allows you to view the console logs, warnings, and errors directly in the browser.

## Usage

To use this script, follow these steps:

1. Clone the repository to your local machine.
2. Open the `index.html` file in a web browser.
3. The console output will be displayed on the page.

## Description

The HTML file in this repository sets up a basic web page that captures console output and displays it in different styles based on the type of message. The following styles are used:

- `log`: Displays regular console log messages in black.
- `warn`: Displays console warning messages in orange.
- `error`: Displays console error messages in red.

The JavaScript code in the `<script>` tags overrides the default behavior of `console.log`, `console.warn`, and `console.error` methods. It saves the original functions and appends the captured messages to the `output` `<div>` on the page.

## Example

The included example in the script demonstrates how the overridden console methods work. It logs a simple message, a warning, an error, and a directory object. The output for each message is displayed below the script.

```javascript
console.log('Hello, console!');
console.warn('This is a warning');
console.error('This is an error');
console.dir({ key: 'value' });

