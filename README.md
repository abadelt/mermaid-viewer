# Mermaid Viewer 

Mermaid Viewer is a simple web application running as as single .html file that allows you to view Mermaid diagrams in your browser. It uses HTML, CSS, and JavaScript to render Mermaid diagrams from text input using the Mermaid library. 

## Purpose

This tool was designed as simple quick solution for an engineering and construction company that needed a way to easily view Mermaid diagrams without needing to set up a complex environment or install additional software. It is lightweight, easy to use, and does not require any server-side processing.

It's not really much of an application at all, just a simple HTML file that you can open in your browser to view Mermaid diagrams. It is designed to be a quick and easy way to visualize diagrams without the need for complex setup or configuration.

## Features 

- Render Mermaid diagrams from text input
- Supports various Mermaid diagram types (flowcharts, sequence diagrams, class diagrams, etc.)
- Responsive design for mobile and desktop
- Easy to use interface
- Example diagrams included
- Single external dependency (Mermaid.js)
- No server required, runs entirely in the browser
- Lightweight and fast
- Themes / Dark Mode support 
- Export diagrams as SVG or PNG (png export requires additional CDN provided library, canvg https://github.com/canvg/canvg)
- Copy diagram text to clipboard

## Download / Installation 

Simplest way to use this tool is to download the `mermaid-viewer.html` file from the repository and open it in your web browser. To do this:
1. Go to the [Mermaid Viewer GitHub repository](https://github.com/KevinOBytes/mermaid-viewer).
2. Click on the `mermaid-viewer.html` file.
3. Click the "Raw" button to view the raw HTML.
4. Right-click and select "Save As" to download the file.

Or download the repository as a ZIP file:

1. Go to the [Mermaid Viewer GitHub repository](https://github.com/KevinOBytes/mermaid-viewer).
2. Click the "Code" button.
3. Select "Download ZIP".
4. Extract the ZIP file to your desired location.


Alternatively, you can clone the repository using Git:

```sh
git clone https://github.com/KevinOBytes/mermaid-viewer.git
```

## Requirements
- A modern web browser (Chrome, Firefox, Safari, Edge, etc.)
- An internet connection to load the Mermaid.js library from the CDN (or you can download it and serve it locally).

## Usage 

1. Open the memrmaid-viewer.html file in your web browser 
    - File > Open File > Select the `mermaid-viewer.html` file.
    - And you can just bookmark the opened file in your browser for easy access (will link to the local saved file).

    Or  
        - Drag and drop the `mermaid-viewer.html` file into your web browser.

    Or  
        - Use a local web server to serve the file (e.g., Python's `http.server`, Node.js, etc.).

    ```sh 
    # This will start a local web server on port 8000.
    python -m http.server 8000
    ```

    Then open your browser and go to `http://localhost:8000/mermaid-viewer.html`.

2. Click the "Load Example" button to load a sample Mermaid diagram.

3. Enter your Mermaid diagram text in the input area.
4. Click the "Render Diagram" button to generate the diagram.
5. Use the "Export SVG" or "Export PNG" buttons to save the diagram.
6. Use the "Copy to Clipboard" button to copy the diagram text.
7. Use the "Dark Mode" toggle to switch between light and dark themes.

## Download Mermaid.js and use it locally 

If you prefer to use Mermaid.js locally instead of loading it from the CDN, you can download it and include it in your project:
1. Download the latest Mermaid.js file from the [Mermaid GitHub releases page](https://github.com/mermaid-js/mermaid/releases).
2. Place the downloaded `mermaid.min.js` file in the same directory as your `mermaid-viewer.html` file.
3. Open the `mermaid-viewer.html` file in a text editor.
4. Find the line that loads Mermaid.js from the CDN:

```html
<script src="https://cdn.jsdelivr.net/npm/mermaid/dist/mermaid.min.js"></script>
```

5. Replace it with a local reference:

```html
<script src="mermaid.min.js"></script>
```

6. Save the changes and open the `mermaid-viewer.html` file in your web browser.

## License 

This is freely licensed under the MIT License, do with it as you please. The code is provided "as is" without warranty of any kind, either expressed or implied.

## Contributing 

This wasn't really developed as a project or intended to be used by anyone outside of the specific company that needed it, but if you find it useful and want to contribute or request features, feel free to open an issue or submit a pull request on the [GitHub repository](https://github.com/KevinOBytes/mermaid-viewer).

## Issues
If you encounter any issues or have suggestions for improvements, please open an issue on the [GitHub repository](https://github.com/KevinOBytes/mermaid-viewer/issues).

## Acknowledgements
This project uses the [Mermaid.js](https://mermaid-js.github.io/mermaid/#/) library for rendering diagrams. Special thanks to the Mermaid.js team for their work on this powerful library.
