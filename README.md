# 🎮 Air Juggler - Webcam Controlled Game

A fun and interactive browser-based game that uses your webcam and hand tracking to control gameplay. Keep the ball in the air by moving your hands in front of the camera!

![Air Juggler Demo](https://img.shields.io/badge/Status-Active-success)
![TensorFlow.js](https://img.shields.io/badge/TensorFlow.js-Enabled-orange)
![License](https://img.shields.io/badge/License-MIT-blue)

## 🌟 Features

- **Real-time Hand Tracking**: Uses MediaPipe Hands via TensorFlow.js for accurate hand detection
- **Webcam-Based Controls**: No keyboard or mouse needed - just use your hands!
- **Physics-Based Gameplay**: Realistic gravity and collision mechanics
- **Visual Feedback**: See your webcam feed with hand tracking overlays
- **Score Tracking**: Track how long you can keep the ball in the air
- **Responsive Design**: Works on desktop browsers with webcam support

## 🚀 Getting Started

### Prerequisites

- A modern web browser (Chrome, Firefox, Edge, Safari)
- A working webcam
- A local web server (required for webcam access)

### Installation

1. Clone this repository:
```bash
git clone https://github.com/yourusername/webcam-controlled-game.git
cd webcam-controlled-game
```

2. Start a local web server. Choose one of these methods:

**Python 3:**
```bash
python -m http.server 8000
```

**Python 2:**
```bash
python -m SimpleHTTPServer 8000
```

**Node.js (http-server):**
```bash
npx http-server -p 8000
```

**VS Code Live Server:**
- Install the "Live Server" extension
- Right-click `index.html` and select "Open with Live Server"

3. Open your browser and navigate to:
```
http://localhost:8000
```

4. Allow webcam access when prompted

## 🎮 How to Play

1. Click the **"Start Game"** button
2. Position yourself in front of your webcam
3. Move your hands to hit the ball and keep it from falling
4. The game tracks your survival time in seconds
5. If the ball hits the ground, game over!
6. Try to beat your high score!

## 🛠️ Technologies Used

- **HTML5 Canvas**: For game rendering
- **JavaScript (ES6+)**: Game logic and physics
- **TensorFlow.js**: Machine learning framework
- **MediaPipe Hands**: Hand tracking model
- **Hand Pose Detection**: TensorFlow.js hand detection library

## 📁 Project Structure

```
webcam-controlled-game/
├── index.html          # Main HTML file
├── game.js             # Game logic and physics
├── handTracking.js     # Hand tracking implementation
├── style.css           # Styling and layout
└── README.md           # This file
```

## 🔧 Configuration

You can customize game parameters by editing the `config` object in `game.js`:

```javascript
const config = {
  ballCount: 1,          // Number of balls (currently supports 1)
  ballRadius: 20,        // Size of the ball
  gravity: 0.05,         // Gravity strength (higher = faster fall)
  bounceVelocity: -4,    // Initial upward velocity when hitting
  handRadius: 50,        // Size of hand detection zone
  countdownTime: 3,      // Countdown before game starts
};
```

## 🔒 Privacy & Security

- All processing happens **locally in your browser**
- Your webcam feed is **never uploaded** to any server
- No data is collected or stored
- Hand tracking runs entirely on your device

## 🐛 Troubleshooting

**Webcam access denied:**
- Make sure you allowed camera permissions in your browser
- Check if another application is using your webcam
- Try refreshing the page and allowing access again

**Hand tracking not working:**
- Ensure good lighting conditions
- Position yourself clearly in front of the camera
- Try moving closer or further from the webcam
- Clear your hands from background clutter

**Performance issues:**
- Close other browser tabs
- Make sure you're using a modern browser
- Check that hardware acceleration is enabled in browser settings

## 🤝 Contributing

Contributions are welcome! Feel free to:
- Report bugs
- Suggest new features
- Submit pull requests

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

## 🙏 Acknowledgments

- [TensorFlow.js](https://www.tensorflow.org/js) - Machine learning in the browser
- [MediaPipe Hands](https://google.github.io/mediapipe/solutions/hands.html) - Hand tracking solution

## 📞 Contact

For questions or feedback, please open an issue on GitHub.

---

**Enjoy playing! 🎮👋**
