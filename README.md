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

## Installation & Usage 🚀 <br/>
1. **Clone the Repository:** <br/>
git clone https://github.com/siddharthpatil-0411/digital-watch.git <br/>

**Create a Directory:** <br/>
mkdir digital-watch <br/>

**Navigate to the Project Directory:** <br/>
cd digital-watch <br/>

**Run the Script:** <br/>
./digital-watch.sh <br/>

**If the script doesn't have execution permissions, you can add them using:** <br/>
chmod +x digital-watch.sh <br/>

**Script Details 🛠️ <br/>
Here's the complete script for the digital watch:** <br/>

#!/bin/bash <br/>
Red=$'\e[1;31m' <br/>
Green=$'\e[1;32m' <br/>
Blue=$'\e[1;34m' <br/>

while true <br/>
do <br/>
       clear <br/>
       echo $Red $(date +%T) <br/>
       sleep 1s <br/>
done <br/>

**How It Works 🧩** <br/>
**Red=$'\e[1;31m'**: This sets the color for the time display to red. <br/>
**while true loop:** The script continuously runs, updating the time every second. <br/>
**clear:** Clears the terminal screen before displaying the updated time. <br/>
**date +%T:** Displays the current time in HH:MM <br/>
format. <br/>
**sleep 1s:** Pauses the script for 1 second before the next update. <br/>
