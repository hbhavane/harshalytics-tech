# 🌸 3D Botanical Lily Animation with Python

A procedural 3D botanical animation of a bouquet of Oriental lilies, created with Python. The animation is designed in a vertical 9:16 format for Instagram Reels.

## ✨ Features

- 🌸 Procedurally constructed 3D lily flowers
- 🌿 Detailed petals, stems, leaves, stamens, and pistils
- 🎬 Animated flower construction and reveal
- 📱 Vertical 1080 × 1920 video format
- 🔒 Password-gated flower reveal with a personal hint
- 🎶 Looping background music with a gramophone play/pause control
- 🐍 Python-based animation generation

## 🛠️ Technologies

- Python
- NumPy
- OpenCV
- Additional Python libraries used by the script

## 📁 Project Structure

```text
lily-animation-python/
├── generate_lily_animation.py
├── index.html
├── assets/
│   └── Sukh-Kalale.mp3
└── lily_frames/
    └── frame_001.webp ... frame_195.webp
```

## 🚀 Getting Started

1. Download or clone this repository.
2. Install the Python dependencies required by the script.
3. Generate or refresh the transparent web animation frames:

```bash
python3 generate_lily_animation.py --web-frames
```

4. Serve the page locally:

```bash
python3 -m http.server 8000
```

Open `http://localhost:8000` in a browser. The page uses transparent WebP frames, so it can layer the bouquet over its animated petal background without a video player.

The welcome screen shows a centered knock-knock hint and asks for the secret phrase. A correct entry plays a brief “YES!” heart-burst before revealing the flower animation. The page attempts to autoplay the looping MP3; browsers that block autoplay start it after the first page interaction. Use the gramophone button to pause or resume playback. Because the password check runs in the page itself, it is a playful gate, not security.

To render the standalone MP4 instead, run `python3 generate_lily_animation.py`.

**Note:** Check the imports at the top of the script and install any required dependencies before running it. MP4 rendering also requires FFmpeg.

## 🎥 Output

The web page reveals a responsive, five-flower lily bouquet over its animated background, followed by draggable floating messages. The script can also generate a vertical MP4.

The thank-you button appears 14 seconds after the letter is opened. Thank-you notes are sent to the configured inbox through Web3Forms. Its public client-side access key is stored in the form's hidden `access_key` field in `index.html`; replace that value if the destination inbox changes.

## 💗 About

Created as a Python animation project exploring procedural botanical modeling and cinematic visual storytelling.

If you found this project through my coding reels, feel free to explore the source code!

---

⭐ If you like this project, consider starring the repository.
