# 🌀 Wormhole Tunnel Rage Simulator (aka "Robot Bobby 3D")

![Wormhole Game](https://img.shields.io/badge/Status-Scientifically%20Questionable-red?style=for-the-badge) ![Three.js](https://img.shields.io/badge/Three.js-Space%20Magic-black?style=for-the-badge&logo=three.js) ![Lasers](https://img.shields.io/badge/Lasers-Pew%20Pew-yellow?style=for-the-badge)

## 🚀 TL;DR  
*Ever wanted to blast wireframe boxes while careening through an infinite red tube in space? No? Well, NOW YOU CAN ANYWAY!*

## 🤔 What Actually Is This?

Welcome to the **Wormhole Tunnel Rage Simulator**—the game nobody asked for but everybody secretly needed. This is a THREE.js-powered space shooter where you're inexplicably trapped in an eternal crimson wormhole, armed with nothing but golden lasers and an existential need to destroy rainbow-colored wireframe cubes.

**The Setup:** You're flying through a looping red tube tunnel in space at a constant speed (because brakes are for cowards). Your mission? Click frantically to shoot glowing laser bolts at randomly-scattered wireframe boxes that are just... floating there. Why are they there? We don't know. Why do they explode into satisfying bloom effects? WHO CARES—IT LOOKS COOL!

**Who's it for?**
- People who miss Star Fox but want less plot
- Developers learning THREE.js who need a dopamine hit
- Anyone with 5 minutes to kill and a mouse
- Fans of tubes, lasers, and questionable physics

## 🛠️ Features

- **🌈 255 Wireframe Boxes of Doom** - Because 254 just wasn't enough chaos
- **💥 Golden Laser Bolts** - Pew pew! (Sound effects sold separately—actually not included at all)
- **🎯 Crosshair That Actually Follows Your Mouse** - Revolutionary technology from 1993
- **✨ UnrealBloomPass Post-Processing** - Making everything look 300% more dramatic than it needs to be
- **🌟 500 Procedurally-Generated Stars** - Each one completely indifferent to your struggle
- **🔴 Infinite Red Tube Prison** - You can't escape. Don't even try. It loops forever.
- **📏 Spline-Based Path** - 39 hardcoded coordinates that definitely weren't just randomly placed
- **🎨 HSL Color Gradient** - Boxes change color based on position because SCIENCE
- **💀 Hit Detection** - Boxes actually disappear when you shoot them (revolutionary, we know)
- **🖱️ Mouse-Controlled Aiming** - Move your mouse. Aim. Click. Repeat until existential crisis.
- **📱 Responsive Design** - Works on any screen size (tunnel of despair scales accordingly)
- **🎭 Two Nearly-Identical Files** - `main.js` AND `dupe.js`—because version control is hard

## 🧑‍💻 How To Install?

### Prerequisites
- Node.js (because nothing runs directly in browsers anymore)
- A mouse (touchpads are for masochists)
- 5 minutes of your life you'll never get back
- Low standards for entertainment

### Installation Steps

1. **Clone this bad boy:**
   ```bash
   git clone https://github.com/RealNickey/Wormhole-game.git
   cd Wormhole-game
   ```

2. **Install dependencies** (aka download half of npm):
   ```bash
   npm install
   ```

3. **Start the dev server:**
   ```bash
   npm run dev
   ```
   
   *Or if you're old-school:*
   ```bash
   npx vite
   ```

4. **Open your browser** to whatever localhost port Vite spits out (probably `http://localhost:5173`)

5. **Embrace the tube.** Let it consume you. You are one with the wormhole now.

## 🎮 How To Play?

1. **Look at the screen** - Red tube. Colorful boxes. Space stuff. Got it? Good.
2. **Move your mouse** - The white crosshair follows you like a loyal puppy
3. **Click to shoot** - Golden lasers go brrrrr
4. **Hit the boxes** - They explode in a glorious bloom of light
5. **Keep shooting** - There's no objective. There's no score. There's only THE VOID.
6. **Experience existential dread** - As you realize the tunnel loops forever and the boxes respawn never

## 📂 Project Structure (aka "Where's The Good Stuff?")

```
Wormhole-game/
├── main.js           # The main event (no bloom effects)
├── dupe.js           # Literally the same thing but with fog and UnrealBloom
├── spline.js         # 39 hardcoded 3D points that define your prison
├── getStarfield.js   # Generates 500 stars that judge your life choices
├── index.html        # 25 lines of HTML that changed everything
├── circle.png        # A circle texture (revolutionary)
├── package.json      # Where dependencies go to party
└── main.txt          # Because someone was too scared to delete old code
```

## 🔧 Technical Deep-Dive (For The Nerds)

**Graphics Magic:**
- THREE.js r0.170.0 (the version number alone adds 10 FPS)
- Perspective Camera with 75° FOV (fish-eye chic)
- ACES Filmic Tone Mapping (makes red look redder)
- Unreal Bloom Pass with strength 3.5 (bloom goes brrr)
- Raycasting for collision detection (actual smart code!)

**The Tube:**
- CatmullRomCurve3 spline with 13 control points
- TubeGeometry with 222 segments (because 200 was too round)
- Radius of 0.65 (scientifically determined by vibes)
- EdgesGeometry for that sweet wireframe aesthetic

**The Boxes:**
- 255 cubes of size 0.075 (tiny but mighty)
- Random rotation on spawn (chaos incarnate)
- HSL color gradient from blue to red (0.7 - p, 1, 0.5)
- Wireframe rendering (because solid cubes are for cowards)

**The Lasers:**
- Icosahedron geometry (fancy word for spiky ball)
- Color: 0xFFCC00 (official hex code for "pew pew yellow")
- Speed: 0.5 units/frame (scientifically calculated)
- Impact explosions scale from 1.0 to infinity (or until opacity dies)

## 🐛 Known Issues (aka "Features")

- ⚠️ **No sound effects** - Your imagination is the sound engine
- ⚠️ **Boxes don't respawn** - Eventually you'll run out of things to shoot (nightmare fuel)
- ⚠️ **No score system** - Your reward is the friends you made along the way (none)
- ⚠️ **dupe.js exists** - We don't talk about dupe.js
- ⚠️ **main.txt lingers** - Like a ghost of commits past
- ⚠️ **Infinite loop** - You can never escape the tube. NEVER.
- ⚠️ **No mobile controls** - Touch controls are for next year
- ⚠️ **Camera auto-flies** - You're just along for the ride, buddy
- ⚠️ **No pause button** - The tube waits for no one

## 🎯 Roadmap (Things That Will Never Happen)

- [ ] Add sound effects (whoosh, pew, boom)
- [ ] Score counter (for competitive tube shooters)
- [ ] Difficulty levels (Easy: 100 boxes, Hard: 1000 boxes, Impossible: ∞ boxes)
- [ ] Power-ups (rapid fire, nuclear lasers, existential immunity)
- [ ] Multiplayer (compete to see who can destroy boxes faster)
- [ ] Boss battles (a really big box?)
- [ ] Story mode (where boxes come from, why you're in a tube)
- [ ] VR support (experience the tube in FULL IMMERSION)
- [ ] Delete dupe.js (probably not happening)
- [ ] Actually use main.txt for something

## 🤝 Contributing

Found a bug? Want to add features? Pull requests welcome! But honestly, this game is perfect as-is—a minimalist masterpiece of pointless destruction.

**How to contribute:**
1. Fork this repo
2. Make it weirder
3. Submit a PR
4. Profit??? (definitely not)

## 📜 License

ISC License (aka "I Sometimes Care" License)

Do whatever you want with this code. Make it better. Make it worse. We believe in you.

## 🙏 Acknowledgments

- **Three.js team** - For making 3D graphics accessible to mere mortals
- **The void** - For inspiration
- **Coffee** - For making this code possible
- **That one Stack Overflow answer** - You know the one
- **The 255 boxes** - Rest in pieces

## 🎬 Credits

**Code:** RealNickey (probably)  
**Art Direction:** Math.random()  
**Sound Design:** Your imagination  
**QA Testing:** YOLO  
**Project Manager:** Procrastination  
**Special Thanks:** Ctrl+C, Ctrl+V

---

## 💭 Final Thoughts

This game answers the age-old question: "What if someone made a Star Fox tunnel level but removed all the fun stuff and added bloom effects?"

The answer is glorious.

Now go forth and shoot those wireframe boxes. They probably deserve it.

*Made with 💥, ☕, and questionable life choices.*

---

**Disclaimer:** No actual robots named Bobby were harmed in the making of this game. The tube is not a real wormhole. Do not attempt to use golden lasers to solve real-world problems.
