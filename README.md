# Flappy Bird - 10 Birds Edition 🐦

A modern, feather-light web reimagining of the classic Flappy Bird arcade game. Built from scratch using native HTML5 Canvas, modern CSS, and vanilla JavaScript—featuring an ultra-floaty physics engine, pure dynamic AudioContext sound synthesis, and 10 uniquely stylized avian skins!

📱 **Play Now on Vercel:** [Live Demo](https://flappybird-drab-eta.vercel.app/) 

## 🚀 Introduction

**Flappy Bird - 10 Birds Edition** brings the classic mobile mechanic right to your web browser with a fresh visual twist. Instead of relying on heavy image assets, every single element—from the procedural clouds and gradient pipes down to the uniquely shaped birds—is rendered dynamically via code.

### Key Features

* 🕊️ **10 Selectable Avian Skins:** Play as a Sparrow, Falcon, Parrot, Owl, Kingfisher, Peacock, Eagle, Dove, Woodpecker, or a rapid-flapping Hummingbird.
* 🎵 **Dynamic Audio Engine:** Sound effects (jump, point, game over) are generated in real-time using the HTML5 Web Audio API (`AudioContext`). No `.mp3` or `.wav` files needed!
* ☁️ **Procedural Backgrounds:** Immersive moving clouds and a high-performance HTML5 Canvas animation loop.
* 🧘 **Ultra-Floaty Physics:** Tuned control settings featuring low gravity and gentle drifting speeds for a more forgiving, strategic gameplay loop.


## 🕹️ How It Works

The entire game runs out of a single file (`index.html`) using raw web standards:

### 1. The Rendering Engine (HTML5 Canvas)

The game utilizes a persistent `requestAnimationFrame` render loop running at your browser's native refresh rate. It clears and redraws elements dynamically based on current coordinates:

* **The Birds:** Drawn procedurally using canvas ellipse and arc methods. The wings feature dynamic scale modifications bound to `Math.sin(Date.now())` to simulate real-time flapping.
* **The Obstacles:** Pipes are rendered using custom linear gradients to give them an authentic, metallic arcade look with precise bounding-box collision parameters.

### 2. The Physics Model

Built with customized kinematic variables to maximize approachability:

* **Feather-Light Gravity:** Set to a low `0.05` to provide a drifting, floaty descent.
* **Smooth Glide:** A jump force of `-2.5` limits jagged mashing, offering fluid upward control.
* **Pacing:** Pipes travel at a slower speed (`1.2`) to allow high-level tactical adjustments.

### 3. Procedural Synthesizer

Audio frequencies are synthesized directly on your sound card:

* **Jump Sound:** Uses a `triangle` oscillator ramping exponentially from `300Hz` to `500Hz` over 0.1 seconds.
* **Score Point:** A dual-tone `sine` wave trigger jumping from `800Hz` to `1200Hz`.
* **Game Over:** A dramatic `sawtooth` pitch drop crushing down to `40Hz`.


## 🛠️ How to Setup & Run Locally

Because this project uses vanilla web standards with zero external dependencies or package builders, setting it up locally takes less than 10 seconds.

### Prerequisites

You only need a modern web browser (Chrome, Firefox, Edge, or Safari).

### Local Installation Steps

1. **Clone the Repository:**
git clone [https://github.com/hemanth-mghr/Flappy_bird.git](https://github.com/hemanth-mghr/Flappy_bird.git)
2. **Navigate to the Project Folder:**
cd Flappy_bird
3. **Launch the Game:**
* Simply double-click the `index.html` file to open it in your default web browser.
* *Alternatively*, if you use VS Code, right-click `index.html` and select **Open with Live Server**.



### Controls

* **Spacebar / Arrow Up** — Flap / Fly upward
* **Left Mouse Click** — Flap / Fly upward
* **Touch Tap (Mobile)** — Flap / Fly upward


## 📜 Credits

* **Game Developer:** Hemanth Naik.M
* **AI Collaborator:** Google Gemini AI
* **Language:** HTML5, CSS3, JavaScript (ES6+)
* **Deployment Platform:** Vercel


## 🎯 Conclusion

This edition of **Flappy Bird** showcases how powerful native web standard APIs have become. By bypassing heavy asset downloads and bulky game engines, the game boasts a microscopic footprint, instantaneous load times, and perfect structural flexibility. Dive in, choose your bird, and try to beat your high score!
