# Digital Watch Script on CentOS 9 🕒
👋 Hi, I'm **SIDDHARTH PATIL**, a DevOps enthusiast diving into the world of Linux and cloud computing. This is my first Linux project, where I've created a simple yet effective digital watch script using shell scripting on CentOS 9.

## Project Overview 📜
In this project, I’ve created a basic shell script that shows a digital clock in the terminal. The time updates every second, and you can change the display color.

## Features ✨
**Real-time Clock:** Shows the current time with hours, minutes, and seconds.
**Colorful Display:** The time appears in red for a nice visual effect.
**Simple and Lightweight:** Requires minimal code and resources.

## Prerequisites 📋
- **Operating System**: CentOS 9 (or any Linux distribution with Bash)
- **Bash Shell**: Installed by default on most Linux systems

## Installation & Usage 🚀
1. **Clone the Repository:**
git clone https://github.com/siddharthpatil-0411/digital-watch.git

**Create a Directory:**
mkdir digital-watch

**Navigate to the Project Directory:**
cd digital-watch

**Run the Script:**
./digital-watch.sh

**If the script doesn't have execution permissions, you can add them using:**
chmod +x digital-watch.sh

**Script Details 🛠️
Here's the complete script for the digital watch:**

#!/bin/bash
Red=$'\e[1;31m'
Green=$'\e[1;32m'
Blue=$'\e[1;34m'

while true
do 
       clear
       echo $Red $(date +%T)
       sleep 1s
done

**How It Works 🧩**
**Red=$'\e[1;31m'**: This sets the color for the time display to red.
**while true loop:** The script continuously runs, updating the time every second.
**clear:** Clears the terminal screen before displaying the updated time.
**date +%T:** Displays the current time in HH:MM
format.
**sleep 1s:** Pauses the script for 1 second before the next update.
