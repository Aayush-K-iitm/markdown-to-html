# Markdown Viewer

A simple, single-page web application designed to dynamically load and render Markdown files (`input.md`) into a clean, responsive HTML view. This project utilizes vanilla JavaScript for Markdown parsing and rendering, enhanced with the power of Tailwind CSS for a modern and adaptable user interface.

## Features

*   **Dynamic Markdown Loading:** Fetches `input.md` from the server and renders its content.
*   **Markdown to HTML Conversion:** Uses the `marked.js` library for efficient and accurate Markdown parsing.
*   **HTML Sanitization:** Incorporates `DOMPurify` to ensure that rendered HTML content is safe and free from potential XSS vulnerabilities.
*   **Responsive Design:** Built with Tailwind CSS, providing a mobile-first and fully responsive layout that looks great on any device.
*   **Clean User Interface:** Presents Markdown content in a readable and aesthetically pleasing format.

## Technologies Used

*   **HTML5:** Standard markup language for creating web pages.
*   **Tailwind CSS:** A utility-first CSS framework for rapidly building custom designs.
*   **JavaScript:** The core programming language for dynamic content and interactivity.
*   **Marked.js:** A fast and powerful Markdown parser and compiler.
*   **DOMPurify:** An XSS sanitizer for HTML, MathML and SVG.

## Setup and Usage

To run this application, simply follow these steps:

1.  **Clone the repository (or save the files):**
    If this were a repository, you'd clone it. For this standalone file, ensure `index.html` and `input.md` are in the same directory.

2.  **Place `input.md`:**
    Make sure your Markdown file, named `input.md`, is located in the same directory as `index.html`. The application is configured to automatically fetch and render this specific file.

3.  **Open `index.html`:**
    Open the `index.html` file in your web browser. The page will automatically load `input.md`, convert its content to HTML, and display it.

    ```bash
    # Example command to open in a browser (macOS)
    open index.html
    ```
    Alternatively, you can serve it via a local web server (e.g., `python -m http.server` in the directory) to ensure `fetch` requests work correctly, especially for `file://` protocol limitations in some browsers.

## Project Structure

```
.
├── index.html        # The main responsive web page
└── input.md          # The Markdown file to be rendered
```

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
