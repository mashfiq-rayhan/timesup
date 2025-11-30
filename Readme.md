# Timer Challenge — Refs Playground Game ⏱️🎯

A small, addictive timing game built with React + Vite. Start a challenge and try to stop the timer as close to 0.00s as possible — but don't let it hit zero, or you lose! 🎮

## How to play 🕹️

- (Optional) Enter your name in the player area and click "Set Name" ✍️
- Pick a challenge and click "Start Challenge" ▶️
- The timer counts down from the challenge's target time — click "Stop Challenge" to stop it ✋
- If you stop close to 0.00s you get a higher score; if it hits zero, you lose 🔥
- Close the result modal to reset and try again 🔁

## Challenges (default) 📋

- Easy — 1 second 🟢  
- Not Easy — 5 seconds 🟡  
- Getting Tough — 10 seconds 🟠  
- Pros Only — 15 seconds 🔴

Try longer targets for a bigger test of precision!

## Scoring 🧮

Score is a percentage representing how close you stopped to 0:
score = round((1 - remainingTime / (targetTime * 1000)) * 100)

- Close to 0 → high score (near 100) 🥇
- Stop early → lower score 🥈
- Hit 0 → loss 💀

## Quick Start 🚀

1. Install dependencies:
```sh
npm install
```

2. Run the dev server:
```sh
npm run dev
```

## Notes ⚠️

- Results use the native <dialog> element rendered into a portal — use a modern browser (Chrome, Edge, recent Firefox) 🪟
- Lightweight demo — great for practicing timing and React refs (useRef + useImperativeHandle) 🧠
