# SignLens – Sign Language Recognition & Real-Time Translation

Browser-based hand-sign recognition. The webcam feed is tracked with MediaPipe Hands (21 hand landmarks), classified into words, shown as text and spoken aloud with the browser's speech synthesis.

## Features
- Live hand tracking from the webcam
- 9 built-in starter signs (Hello, Yes, Good, I love you, Peace, You, Call me, I, OK)
- **Teach a sign:** record your own signs; a k-nearest-neighbour classifier on landmark data recognises them (stored in localStorage)
- Hold-to-confirm (about half a second) to avoid false words
- Text translation with Speak, Undo and Clear
- Fully on-device: no video or data is uploaded

## Run locally
`npx serve .` or `python3 -m http.server 3000` (camera needs `localhost` or `https`).

## Deploy
GitHub: upload all files. Vercel: import the repo, Framework = Other, no build command.

## Limitations
- Starter signs are static hand shapes, not full ASL/BdSL/ISL, which also use motion and facial expression.
- One hand at a time. Custom signs work best when recorded by the person who will use them.
- Future scope: sequence model (LSTM/Transformer) for moving signs, two-hand support, language packs.

Made by Sudipto Acharjee Dhrubo
