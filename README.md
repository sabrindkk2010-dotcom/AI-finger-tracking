# Finger Tracking Project
## Motivation
Designed this project in PictoBlox to track finger movements and identify patient needs, aiming to help caregivers monitor patients more efficiently.
## Features
- Tracks finger movements to detect and identify patients' needs.
- Provides real-time feedback to assist caregivers or medical staff.
- Can be adapted to different patient monitoring scenarios
## Tech Stack
- **Platform / Framework:** PictoBlox (block-based programming)
- **Programming Style:** Visual coding, drag-and-drop blocks
- **Libraries / Extensions Used:** Scratch-based extensions (e.g., Motion, Sound, Pen, Sensors)
## Installation
1. Install **PictoBlox** from [https://thestempedia.com/product/pictoblox/](https://thestempedia.com/product/pictoblox/)  
2. Open PictoBlox and recreate the project using the block descriptions provided beneath
## Block Descriptions
This section explains how the finger-tracking patient assistance project works in PictoBlox.
### 1. Start the Project
- **Event Block:** `When green flag clicked`
- **Action:** Turn on video on stage with 0% transparency  
- Initializes the webcam and prepares the project for monitoring.
### 2. Detect Patient Conditions
The project continuously monitors the video feed to identify patient conditions:
1. **Accelerated Heartbeat**
   - **Condition Block:** `if is identified class from web camera in accelerated heartbeat?`
   - **Response:** Displays a message: “Stay calm, and don’t move too much until the doctor is here” for 2 seconds
2. **High/Low Blood Pressure**
   - **Condition Block:** `if is identified class from web camera in blood pressure: high/low?`
   - **Response:** Displays: “Please drink a cup of water… your case was sent, the doctors will be right here” for 2 seconds
3. **Diabetes**
   - **Condition Block:** `if is identified class from web camera in diabetes?`
   - **Response:** Displays: “Please sit down and don’t move, take a deep breath, the doctors are on their way to you” for 2 seconds
4. **Hypoxia (lack of oxygen)**
   - **Condition Block:** `if is identified class from web camera in Hypoxia?`
   - **Response:** Displays: “It’s okay, the most important thing is to stay calm… the doctors will be here in a few secs” for 2 seconds
5. **Unknown / No Condition Detected**
   - **Condition Block:** `if is identified class from web camera in null?`
   - **Response:** Asks the patient: “How can I help you?” and waits for input
## Demo
Here’s how the project looks in PictoBlox:

<img width="300" height="500" alt="code" src="https://github.com/user-attachments/assets/8b5be227-5827-4a5f-aa7c-bdeaed4b89f5" />

