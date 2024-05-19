# Webform Page

This repository contains a simple HTML page that embeds a Google Form within an iframe. The HTML file (`index.html`) is designed to be minimalistic and user-friendly, providing a clean interface for users to fill out the form.

## Files

- `index.html`: The main HTML file that displays the webform.

## index.html

The `index.html` file includes the following structure and styling:

### Structure

- **DOCTYPE and HTML tags**: Defines the document type and root element.
- **Head section**: Contains meta information and the title of the page.
- **Body section**: Contains a centered container with a heading and an iframe.

### Styling

The page uses simple CSS styles for a clean and responsive design:

- **Body**: Flexbox layout to center the content vertically and horizontally, with a light background color.
- **Heading**: Styled with a dark color.
- **Form container**: A white background with padding, rounded corners, and a subtle shadow to give it a card-like appearance.
- **Iframe**: Full width of the container and a fixed height, with no borders.

### Example

Here’s a preview of the `index.html` file:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Webform</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            height: 100vh;
            background-color: #f0f0f0;
        }
        h1 {
            color: #333;
        }
        .form-container {
            width: 80%;
            max-width: 700px;
            padding: 20px;
            background-color: #fff;
            box-shadow: 0 2px 4px rgba(0,0,0,0.1);
            border-radius: 8px;
            text-align: center;
        }
        iframe {
            width: 100%;
            height: 443px;
            border: none;
        }
    </style>
</head>
<body>
    <div class="form-container">
        <h1>Webform</h1>
        <iframe src="https://docs.google.com/forms/d/e/1FAIpQLSfdziIjG9VxnXqU273gwveREsdAD61JpEOmbrKY922lHpyVDw/viewform?embedded=true" 
                width="640" 
                height="443" 
                frameborder="0" 
                marginheight="0" 
                marginwidth="0">
            Loading…
        </iframe>
    </div>
</body>
</html>
