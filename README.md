# 3D Photo Viewer with Face Tracking

A web-based application that converts 2D images into interactive 3D views controlled by face movements. This project combines depth estimation, face tracking, and 3D rendering to create an immersive viewing experience.

![Depth Map Preview](/images/screen-2.png)


## Features

- **Real-time Face Tracking**: Uses your webcam to track face movements and control the camera view
- **Depth Map Generation**: Converts 2D images into 3D using AI-powered depth estimation
- **Interactive Controls**: Fine-tune the experience with an intuitive control panel
- **Mobile-Ready**: Optimized for iOS web app installation with proper status bar handling
- **Dark Theme**: Modern dark interface with blur effects and rounded corners

## How It Works

1. **Depth Estimation**
   - Uses Pydnet (TensorFlow.js) to generate depth maps from 2D images
   - Processes images in real-time with WebGL acceleration
   - Visualizes depth information in a preview window

2. **Face Tracking**
   - Utilizes BlazeFace for real-time face detection
   - Tracks face position through webcam feed
   - Translates face movements into camera controls

3. **3D Rendering**
   - Employs Three.js for 3D scene management
   - Applies depth maps as displacement maps on 3D meshes
   - Uses custom shaders for rounded corners and edge effects

![Application Interface](/images/screen-1.png)



## Controls

### Face Tracking Controls
- **X Sensitivity**: Adjust horizontal movement sensitivity (0.1-3.0)
- **Y Sensitivity**: Adjust vertical movement sensitivity (0.1-3.0)
- **Smoothing**: Control camera movement smoothness (0.01-0.5)
- **Camera Distance**: Adjust view distance (0.5-3.0)
- **Invert Camera**: Toggle movement direction

### Image Controls
- **Select Image**: Choose from preset images
- **Load Selected Image**: Apply selected image
- **Upload Custom Image**: Process your own images

## Technical Details

### Technologies Used
- **TensorFlow.js**: AI model execution in browser
- **Three.js**: 3D graphics rendering
- **BlazeFace**: Face detection and tracking
- **WebGL**: Hardware-accelerated graphics
- **dat.GUI**: Control interface

### Performance Optimizations
- Efficient shader-based rendering
- Optimized face tracking loop
- Smart texture management
- Smooth camera interpolation

## Installation

1. Clone the repository
2. Host on a web server (required for webcam access)
3. Access through a WebGL-enabled browser

## Usage

1. Allow webcam access when prompted
2. Select an image from the preset options or upload your own
3. Move your face to control the 3D view:
   - Left/Right: Rotate horizontally
   - Up/Down: Rotate vertically
4. Adjust controls as needed for optimal experience

## Image Credits
Danny Ruchtie abd Unsplash

Sample images provided by [Unsplash](https://unsplash.com)
- Example images used under the Unsplash License

## Browser Support

- Chrome (recommended)
- Firefox
- Safari
- Edge (Chromium-based)

Requires:
- WebGL support
- WebRTC (for webcam)
- Modern JavaScript features

## Known Limitations

- Requires good lighting for face tracking
- Performance depends on device capabilities
- Some browsers may limit webcam access

## Future Improvements

- Additional depth estimation models
- More image effects and filters
- Performance optimizations
- Mobile gesture controls
- Batch processing support

## License

[Your chosen license]

## Acknowledgments

- TensorFlow.js team for the ML capabilities
- Three.js community for 3D rendering
- Unsplash for sample images
- [Other acknowledgments]
