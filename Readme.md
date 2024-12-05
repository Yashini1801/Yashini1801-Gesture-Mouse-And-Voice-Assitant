## Gesture-Mouse-Voice-Assistant

A Python-based virtual assistant combining gesture recognition, mouse control, and voice-based interaction. This project enhances user productivity and accessibility by integrating voice commands, gesture recognition, and system control features.

Note: Use Python version: 3.8.5


---

## 🚀 Features
- **Voice Assistant**: Perform system tasks, search the web, and interact with applications via voice commands.
- **Gesture Recognition**: Control mouse movements and system actions using hand gestures.
- **System Automation**: Copy, paste, open files, and navigate directories with simple voice or gesture commands.
- **Proton Personality**: Your AI assistant "Proton" can greet, respond, and provide assistance.

---

## 🛠️ Installation

Follow these steps to set up the project on your local machine:

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/Gesture-Mouse-Voice-Assistant.git
   cd Gesture-Mouse-Voice-Assistant
   ```

2. Create and activate the virtual environment:
   ```bash
   conda create --name gest python=3.8.5
   conda activate gest
   ```

3. Install the dependencies:
   ```bash
   pip install -r requirements.txt
   pip install opencv-python
   ```

4. Install additional libraries:
   ```bash
   conda install PyAudio
   conda install pywin32
   ```

5. Navigate to the source directory:
   ```bash
   cd to till src folder
   ```
   Command may look like: cd C:\Users\.....\Gesture-Controlled-Virtual-Mouse\src

6. Run the project:
   ```bash
   python Proton.py
   ```

( You can enable Gesture Recognition by using the command "Proton Launch Gesture Recognition" )

Or to run only Gesture Recognition without the voice assisstant:

Uncomment last 2 lines of Code in the file Gesture_Controller.py

```bash
   python Gesture_Controller.py
   ```

---

## 📋 Requirements

- Python 3.8.5
- **Conda** (for virtual environment management)
- Required Python libraries:
  - `opencv-python`
  - `PyAudio`
  - `pywin32`
  - Additional dependencies from `requirements.txt`

---

## 🖥️ Usage

### **Mouse Control via Hand Gestures**
1. **Move Mouse Cursor**:  
   - **Gesture**: Move your hand in the air while keeping the palm open.  
   - **Function**: Moves the mouse cursor across the screen according to your hand's position.

2. **Left Click**:  
   - **Gesture**: Show a closed fist and release it quickly (or similar predefined gesture).  
   - **Function**: Simulates a left mouse button click.

3. **Right Click**:  
   - **Gesture**: Show a specific finger gesture (e.g., two fingers forming a "V").  
   - **Function**: Simulates a right mouse button click.

4. **Scroll Up**:  
   - **Gesture**: Move your hand upward while keeping fingers extended.  
   - **Function**: Scrolls the screen or page upward.

5. **Scroll Down**:  
   - **Gesture**: Move your hand downward while keeping fingers extended.  
   - **Function**: Scrolls the screen or page downward.

### **Gesture-Based System Controls**
1. **Zoom In**:  
   - **Gesture**: Move two fingers apart (spread gesture).  
   - **Function**: Performs a zoom-in action (e.g., pinch zoom-in for images or maps).

2. **Zoom Out**:  
   - **Gesture**: Move two fingers closer (pinch gesture).  
   - **Function**: Performs a zoom-out action.

3. **Volume Control**:  
   - **Gesture**: Move your hand left/right or upward/downward with a specific posture.  
   - **Function**: Adjusts the system volume (increase or decrease).

### **Static Controls**:
1. **Greet Proton**:  
   - Command: `hello`  
   - Response: Greets you with a suitable greeting based on the time of day.

2. **Get Proton's Name**:  
   - Command: `what is your name`  
   - Response: "My name is Proton!"

3. **Ask for the Date**:  
   - Command: `date`  
   - Response: Provides the current date.

4. **Ask for the Time**:  
   - Command: `time`  
   - Response: Provides the current time.

5. **Search the Web**:  
   - Command: `search [query]`  
   - Example: `search Python tutorials`  
   - Response: Opens a Google search for the specified query.

6. **Find a Location**:  
   - Command: `location`  
   - Response: Prompts you to say the name of a place, then opens Google Maps to locate it.

7. **Goodbye**:  
   - Commands: `bye`, `by`  
   - Response: "Goodbye! Have a nice day." (Sets Proton to sleep mode.)

8. **Exit the Program**:  
   - Commands: `exit`, `terminate`  
   - Response: Exits the program completely.

---

### **Dynamic Controls**:
1. **Launch Gesture Recognition**:  
   - Command: `launch gesture recognition`  
   - Response: Activates the gesture recognition feature.

2. **Stop Gesture Recognition**:  
   - Commands: `stop gesture recognition`, `top gesture recognition`  
   - Response: Deactivates the gesture recognition feature.

3. **Copy Text**:  
   - Command: `copy`  
   - Response: Simulates a keyboard copy command (`Ctrl + C`).

4. **Paste Text**:  
   - Commands: `paste`, `page`, `pest`  
   - Response: Simulates a keyboard paste command (`Ctrl + V`).

---

### **File Navigation**:
1. **List Files in Root Directory**:  
   - Command: `list`  
   - Response: Lists all files and directories in the root directory (`C://`).

2. **Open File or Folder**:  
   - Command: `open [file number]`  
   - Example: `open 1`  
   - Response: Opens the specified file or folder from the listed directory.

3. **Go Back to the Previous Folder**:  
   - Command: `back`  
   - Response: Navigates back to the parent directory.

---

### **Other Commands**:
1. **Wake Up Proton**:  
   - Command: `wake up`  
   - Response: Wakes up Proton from sleep mode.

2. **Unhandled Commands**:  
   - Any command Proton doesn't recognize results in:  
     - Response: "I am not functioned to do this!"

---

## 📂 Project Structure

```plaintext
Gesture-Mouse-Voice-Assistant/
│
├── src/
│   ├── Proton.py                 # Main Python script
│   ├── Gesture_Controller.py     # Gesture recognition logic
│   ├── app.py                    # Chatbot GUI and communication module
│   └── requirements.txt          # Dependencies
│
├── README.md                     # Documentation file
├── LICENSE                       # Project license
└── .gitignore                    # Files and directories to ignore in Git
```

---

## 🎨 Key Technologies

- **OpenCV**: For implementing gesture recognition.
- **SpeechRecognition**: To capture and process voice commands.
- **Pyttsx3**: For text-to-speech conversion.
- **PyAudio**: For real-time microphone input.
- **PyWin32**: For Windows-specific functionality.

---
