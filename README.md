# 3D Photo Viewer with Depth Estimation

A browser-based application that creates interactive 3D visualizations from 2D images using AI-powered depth estimation. The application runs entirely in your browser, using TensorFlow.js for depth estimation and Three.js for 3D rendering.

## Features

- Browser-based 3D conversion (no server uploads needed)
- Real-time depth map generation using TensorFlow.js and MobileNet
- Interactive 3D model with mouse controls:
  - Click and drag to rotate the model
  - Automatic rotation when not interacting
- Live depth map preview
- Responsive design that adapts to your screen size
- WebGL-powered 3D rendering

## Technical Details

The application uses:
- **TensorFlow.js** (v1.7.4) for AI-powered depth estimation
- **MobileNet** (v1.0.0) for feature extraction
- **Three.js** (r128) for 3D rendering
- Pure client-side JavaScript implementation
- WebGL for hardware-accelerated graphics

## Running the Application

You can run the website using any of these simple server methods:

### 1. Using Python

```bash
# If you have Python 3:
python -m http.server 8000

# If you have Python 2:
python -m SimpleHTTPServer 8000
```
Then visit: `http://localhost:8000`

### 2. Using Node.js

First install a server package:
```bash
# Using npx (comes with Node.js)
npx serve

# Or using http-server
npm install -g http-server
http-server
```
Then visit the URL shown in the terminal (usually `http://localhost:8080`)

### 3. Using PHP

```bash
php -S localhost:8000
```

### 4. Using Visual Studio Code

Install the "Live Server" extension and right-click on `index.html` -> "Open with Live Server"

## How to Use

1. Start any of the servers mentioned above
2. Open your browser and navigate to the local server URL
3. Click "Choose File" to select an image
4. Click "Process & View in 3D" to generate the 3D visualization
5. Use your mouse to interact with the 3D model:
   - Click and drag to rotate
   - The model will auto-rotate when not being manipulated

## Limitations

- Works best with images that have clear foreground/background separation
- Processing time may vary depending on image size and device capabilities
- Depth estimation is an approximation and may not be perfect for all images

## License

This project is licensed under the Apache License 2.0 - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- TensorFlow.js team for the machine learning capabilities
- Three.js team for the 3D rendering engine
- MobileNet contributors for the neural network architecture