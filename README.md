🤖 Wakeup AI Assistant
Conquer your professional interviews with real-time, discreet AI assistance.

Wakeup AI Assistant is a specialized Windows overlay application designed to provide instant, concise answers and detailed explanations during high-stakes remote interviews. It uses the Gemini API for ultra-fast, contextual assistance, ensuring you never miss a beat.

✨ Key Features
Feature

Icon

Description

Real-Time Transcription

🎙️

Captures interviewer's questions from system audio ('Stereo Mix') or your microphone and displays them instantly.

Dual-Tier AI Answers

💬

Trigger Standard (concise, point-form) answers with Enter/Tab, or Detailed Continuation (comprehensive follow-up) with Ctrl+Enter.

Discreet Overlay

🌁

Fully adjustable transparency and topmost window settings, ensuring it remains visible but unobtrusive during webcam use.

Rapid Controls

⌨️

Instantly Hide/Restore (F1) the window and quickly Toggle Audio Input (F2) between your mic and system audio for seamless use.

License Management

🔑

Tracks free usage (20 responses/day) and provides an in-app path for Pro License activation for unlimited use.

🛠️ Installation & Setup (Windows)
The Wakeup AI Assistant requires a Python environment and is specifically designed for the Windows operating system.

Prerequisites
Python: Python 3.9+ installed.

Dependencies: Install required libraries.

pip install google-genai tkinter speechrecognition pystray Pillow requests pyinstaller

External Tool: The external tool nircmd.exe must be present in the same directory as the script/executable to manage the default audio input device.

API Key: Set your Gemini API key as an environment variable:

# In Windows Command Prompt:
set GEMINI_API_KEY="YOUR_API_KEY_HERE"

Running the Application
For a clean execution without the command console:

Direct Execution (Developer Mode):

python wakeup_assistant.py

Executable Distribution (Recommended):
If you are distributing the application, package it using PyInstaller:

pyinstaller --onefile --noconsole --name "WakeupAssistant" wakeup_assistant.py

The final executable will be located in the dist/ folder. Remember to distribute the nircmd.exe alongside the executable.

🚀 Hotkeys & Core Usage
Hotkey/Action

Function

Resulting AI Answer

F1

Hide/Restore main window.

-

F2

Toggle Audio Input (Mic Array ↔ Stereo Mix).

-

ENTER / TAB

Submits current question input.

Standard Answer (Concise Points)

CTRL + ENTER

Submits last question for deeper analysis.

Detailed Continuation (Comprehensive Explanation)

🌐 Landing Page & Demo
This repository also contains the static landing page for the product.

File: index.html

Deployment: The landing page is a single, static HTML file utilizing Tailwind CSS, making it easy to deploy to services like GitHub Pages, Netlify, or Vercel.

Live Demo / Official Website (Update this link after deployment)

✉️ Contact
For licensing inquiries, support, or feedback, please contact:

Email: support@wakeupai.com

License Activation: Use the in-app registration dialog to send your Machine ID.
