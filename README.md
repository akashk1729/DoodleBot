# DoodleBot

DoodleBot is a creative embedded systems project where a wheeled robot equipped with a touch-enabled LCD screen draws vectorized images or user input. The project combines concepts from motion control, image processing, PID tuning, and hardware-software integration, offering an engaging and hands-on introduction to robotics and mechatronics.

This repository contains all code, documentation, and resources required to build, control, and extend DoodleBot.

---

## Mentors

- **Ashish Upadhyay**
- **Bhuvan Kumar KP**
- **Dhakshith Sureshkumar** 
- **Mrigeesh Ashwin**
  
For doubts, discussions, or collaboration, feel free to reach out to the mentors via Discord/email.

---
## Hardware Requirements

| Component                       | Description                                                                 |
|--------------------------------|-----------------------------------------------------------------------------|
| **Raspberry Pi 4** | Central controller handling GUI, CV, and bot control logic             |
| **Wheeled Chassis with DC Motors** | 2-wheel or 4-wheel drive platform for movement                          |
| **Motor Driver (L298N / L9110S)** | For driving DC motors from Pi or external microcontroller               |
| **Camera Module (e.g., Pi Cam v2 / USB Webcam)** | Mounted to track bot’s movement/drawings                  |
| **Touch-enabled LCD Display** | For user input or displaying drawing content          |
| **Power Supply**                | 5V/3A for Raspberry Pi, separate 6–12V supply for motors (if needed)      |
| **Reflective markers / ArUco tags** | For visual tracking and position estimation (used in CV loop)         |
| **Wheels, Castor, Frame**       | Basic robotics platform build (can be 3D printed or sourced externally)   |

---

## Software Requirements

Install the following tools and Python libraries:

### Python Libraries

Create a `requirements.txt` and install using:
```bash
pip3 install -r requirements.txt

### Cloning the Repo
git clone https://github.com/MrigeeshAshwin/doodlebot.git
cd doodlebot
