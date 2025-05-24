# Cosmic Music Visualizer

This project contains two HTML files, `claude4.html` and `gemini2.5pro.html`, both designed to visualize audio. They offer different levels of complexity and features for a "Cosmic Music Visualizer" experience.

## How to Run

To view these HTML files locally, you need a simple web server. The easiest way to do this is by using `serve`, a static file serving utility for Node.js.

1.  **Install Node.js and npm:** If you don't have Node.js and npm (Node Package Manager) installed, download and install them from [nodejs.org](https://nodejs.org/).
2.  **Install `serve`:** Open your terminal or command prompt and run the following command to install `serve` globally:
    ```bash
    npm install -g serve
    ```
3.  **Start the server:** Navigate to the directory where your `claude4.html` and `gemini2.5pro.html` files are located (e.g., `c:/Users/USER/Desktop/vibecodetest`) and run:
    ```bash
    serve
    ```
    This will start a local web server, typically accessible at `http://localhost:3000`.
4.  **Open in browser:** Open your web browser and navigate to:
    *   `http://localhost:3000/claude4.html`
    *   `http://localhost:3000/gemini2.5pro.html`

## `claude4.html` - Simple Music Visualizer

This file provides a basic music visualizer.

### Features:
*   **Audio Upload:** Allows users to upload an audio file (MP3, WAV).
*   **Basic Visualization:** Displays a visual representation of the uploaded audio.

### Usage:
1.  Open `claude4.html` in your browser.
2.  Click the "Choose Audio File" button to select an audio file from your computer.
3.  The visualization will start automatically once the audio begins playing.

## `gemini2.5pro.html` - Advanced Music Visualizer

This file offers a more feature-rich music visualizer with multiple visualization modes and color schemes.

### Features:
*   **Audio Upload:** Upload MP3 or WAV audio files.
*   **Play/Pause & Volume Control:** Standard audio playback controls.
*   **Seek Bar:** Navigate through the audio track.
*   **Fullscreen Mode:** View the visualizer in fullscreen.
*   **Multiple Visualization Modes:**
    *   **Waveform:** Displays the audio waveform.
    *   **Spectrum:** Shows the frequency spectrum of the audio.
    *   **Particles:** Generates dynamic particle effects based on audio.
    *   **3D Shapes:** (Requires WebGL) Renders interactive 3D objects that react to audio frequencies.
*   **Color Schemes:** Choose from predefined color palettes (Neon Glow, Cosmic Fire, Aurora Borealis, Star Dust) to customize the visualizer's appearance.

### Usage:
1.  Open `gemini2.5pro.html` in your browser.
2.  Click the "Choose File" button to select an audio file.
3.  Use the play/pause button to control playback.
4.  Adjust volume and seek through the track using the respective sliders.
5.  Experiment with different "Modes" and "Colors" to change the visualization style.

### Notes:
*   **WebGL Requirement for 3D Shapes:** The "3D Shapes" visualization mode requires WebGL support in your browser. If WebGL is not available or enabled, this mode will be disabled, and a message will be displayed.
*   **Tailwind CSS Warning:** You might see a console warning about `cdn.tailwindcss.com` not being for production. This is expected as Tailwind CSS is included via CDN for simplicity in this local demonstration.
*   **Favicon 404:** A "Failed to load resource: the server responded with a status of 404 (Not Found)" error for `favicon.ico` is normal and does not affect the visualizer's functionality.

## Technologies Used:
*   **HTML5:** Structure of the web pages.
*   **CSS3 (with Tailwind CSS via CDN):** Styling and layout.
*   **JavaScript:** Core logic for audio processing, visualization, and UI interaction.
*   **Web Audio API:** For audio analysis and processing.
*   **Three.js:** (Used in `gemini2.5pro.html`) A JavaScript 3D library for rendering 3D graphics.
