# Automatic Page Redirect Script

This script redirects users to a specified page after a set delay (7 seconds by default). It’s useful for pages that require an automatic redirect after a few seconds.

## Features

- Redirects users to another page after a specified delay (default: 7 seconds).
- Simple and customizable.

## How to Use

1. **Copy the following HTML code** into a new HTML file:

    ```html
    <!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta http-equiv="X-UA-Compatible" content="IE=edge">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Page Redirect</title>
        <script>
            // Function to redirect the page after a 7-second delay
            function redirectAfterDelay() {
                setTimeout(function() {
                    window.location.href = "https://example.com"; // Replace with the target URL
                }, 7000); // 7000 ms = 7 seconds
            }
        </script>
    </head>
    <body onload="redirectAfterDelay()">
        <h1>You will be redirected in 7 seconds...</h1>
    </body>
    </html>
    ```

2. **Set the Target URL**:

    - Replace `https://example.com` in the `window.location.href` line with the desired target URL.

3. **Adjust the Redirect Delay** (optional):

    - Change `7000` (7 seconds) in the `setTimeout` line if you’d like a different delay.

4. **Save and open the HTML file** in a browser to test the automatic redirect.

## Notes

- Ensure JavaScript is enabled in the browser for the redirect to work properly.
- This script is ideal for introductory pages, splash pages, or notices that need a time delay before redirecting.

## License

This project is licensed under the [MIT License](LICENSE).
