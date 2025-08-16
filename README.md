# Two-in-One Image Combiner

A web application that allows you to combine two images vertically with advanced editing features, making it easy to create print-ready images (especially for A4 paper).

## Overview

This tool enables users to:

- **Upload or Scan Images**: Use file inputs to upload images or capture them using your device's camera. The app offers document scanning with automatic edge detection and perspective correction using OpenCV.js.
- **Edit Images**: Rotate images in 90° increments and crop them interactively via a canvas-based interface.
- **Combine Images**: Vertically stack two images while ensuring they are resized to the same width, preserving aspect ratios.
- **A4 Page Fitting**: Optionally fit the combined image onto an A4 canvas (portrait) with customizable DPI, margins, and slider-controlled positioning.
- **Download**: Save the final combined image as a high-quality JPEG file ready for printing or sharing.

## Features

- **Responsive Design**: Works on both mobile and desktop browsers. The layout adapts automatically using CSS media queries.
- **Interactive Editing**: Use rotation and cropping tools to fine-tune the images before combining them.
- **Document Scanning**: Leverages OpenCV.js to detect and correct document edges, ensuring scans capture only the document.
- **Customizable Output**: Adjust output resolution (DPI), margins, and image positioning on an A4 canvas.

## Installation

1. **Clone the Repository**
   ```bash
   git clone https://github.com/priyanshugusain2004/twoinone.git
   cd twoinone
   ```

2. **Open in VS Code**
   Open the folder in VS Code to edit and run the project (it works in a standard web environment).

3. **Run the App**
   Simply open the `index.html` file in your preferred web browser. For local camera scanning, using `localhost` or HTTPS is recommended.

## Usage

1. **Upload/Scan Images**
   - Upload two images via the provided input fields or use the "Scan with camera" option to capture images directly. For the scanning feature, ensure your browser supports camera access, and if on HTTP, note that some features may require HTTPS or `localhost`.

2. **Edit Images**
   - Rotate the images using the provided rotate buttons.
   - Crop images by dragging over the preview canvas.

3. **Combine and Fit**
   - Click the "Combine" button to merge the images vertically.
   - Use the A4 options to fit the output on an A4 page, set DPI, and adjust the image position using sliders.

4. **Download**
   - After combining, click "Download JPEG" to save the final output.

## OpenCV.js Integration

The application uses [OpenCV.js](https://docs.opencv.org/4.x/) for document scanning. OpenCV is loaded asynchronously and enhances captured images by automatically detecting document edges and applying perspective correction.

## Troubleshooting

- **Camera Access**: Ensure that you use HTTPS or `localhost` for camera access as many browsers restrict this feature on non-secure origins.
- **Edge Detection**: If document scanning doesn’t work as expected, try adjusting lighting conditions or use the fallback cropping mechanism.

## Contributing

Contributions are welcome! Feel free to fork the repository and submit pull requests with improvements or bug fixes.

## License

This project is open-source. See the [LICENSE](LICENSE) file for details.

## Acknowledgements

- Thanks to the OpenCV.js team for their robust computer vision library, which powers the document scanning feature.
- Inspired by the needs of users wanting an easy tool to combine images for print.
