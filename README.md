
# 🎮 Real Life Simulation Game – Motion-Controlled NES Gameplay

This project is a real-life simulation interface that allows players to control **NES gameplay** using their **body movements** via webcam. It uses **MediaPipe Pose Estimation** to track posture in real time and maps physical gestures to in-game actions like **jumping**, **shooting**, and **moving forward** — offering a fun and immersive experience.

---

## 🕹️ How It Works

- Uses **MediaPipe Pose** to track full-body movements from the webcam.
- Converts specific gestures (like moving hands or jumping) into **keyboard commands**.
- Sends those keys to the **Running NES game in FCEUX emulator**.
- No manual controller needed — **your body is the controller**!

---

## 🤖 Technologies Used
- Python
- OpenCV
- NumPy
- pyautogui
- MediaPipe
- matplotlib (for temporary debug visuals)

# 🎮 Game Setup (Step-by-Step)

## 1️⃣ Download FCEUX Emulator
Go to the official website:  
👉 https://fceux.com/web/home.html
- Download the appropriate version for your system (Windows/Linux)  
- Extract or install it on your computer

## 2️⃣ Get a NES Game File
- Find and download a `.nes` file (e.g., `contra.nes`)  
- **Note:** We used Contra for this project  
- You can also try other `.nes` game files  
  
## 3️⃣ Setup the Game in FCEUX
- Open FCEUX  
- Go to `File → Open ROM` and select `.nes` file  
- Open `Config → Input` and set keyboard keys:
  - Map `j` for **Jump**
  - Map `s` for **Shoot**
  - Map `d` for **Move Right**

---

# ▶️ How to Run the Project

## Step 1: Install Required Libraries
Open a terminal and run:
``bash
pip install opencv-python mediapipe pyautogui numpy matplotlib

## Step 2: Launch Emulator
Open FCEUX and run the contra.nes file
Leave the emulator window open

## Step 3: Run the Python File
--bash
python main.py

## Step 4: Play with Your Body!
Stand in front of the webcam (entire body visible)
Use these gestures:
Jump in place → triggers j key (in-game jump)
Move your body forward/back → triggers d (move forward)
Bring hands together → triggers s (shoot)

🧠 The script tracks your pose in real-time and maps movements to game commands using pyautogui.







