🚀 **Week 0: VLSI System Design (VSD) Program Foundation & Tool Setup**
https://camo.githubusercontent.com/4e5c13cc756734e4c9031790737bf07c5f67d25e1817a51dd99521b35c6a9098/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f564c53492d53797374656d25323044657369676e2d626c75653f7374796c653d666f722d7468652d6261646765266c6f676f3d63686970

📌 VLSI Week 0 Status

Welcome to my VLSI System Design (VSD) Program repository!
This week was all about setting up the development environment and installing the essential open-source tools that will be used throughout the program. The goal was to create a reliable and efficient workspace for synthesis, simulation, and design tasks.

🎯 **System and Virtual Machine Configuration**

Specification 💻	Details 📋
Operating System 🐧	Ubuntu 20.04+
RAM 💾	6GB
Storage 💿	50GB HDD
vCPUs ⚡	4

💡 Pro Tip: This setup ensures smooth handling of toolchains and simulations.

⚙️ **Tool Installation & Verification**

The following open-source tools were installed for RTL synthesis, simulation, circuit analysis, and layout design:

🧠 Yosys – RTL Synthesis

📟 Iverilog – Verilog Simulation

📊 GTKWave – Waveform Analysis

⚡ Ngspice – Circuit Simulation

🎨 Magic VLSI – Layout Design

🧠 Yosys – RTL Synthesis Tool

Purpose: Converts RTL code into gate-level representations.

# Clone Yosys
git clone https://github.com/YosysHQ/yosys.git
cd yosys 

# Install dependencies
sudo apt install make build-essential clang bison flex \
libreadline-dev gawk tcl-dev libffi-dev git \
graphviz xdot pkg-config python3 \
libboost-system-dev libboost-python-dev \
libboost-filesystem-dev zlib1g-dev

# Build & Install
make 
sudo make install


✅ Yosys Successfully Installed


📟 Iverilog – Verilog Simulator
sudo apt-get install iverilog


✅ Iverilog Successfully Installed

📊 GTKWave – Waveform Viewer
sudo apt update
sudo apt install gtkwave


✅ GTKWave Successfully Installed

⚡ Ngspice – Circuit Simulator
sudo apt update
sudo apt install ngspice


✅ Ngspice Successfully Installed

🎨 Magic VLSI – Layout Tool
# Install dependencies
sudo apt-get install m4 tcsh csh libx11-dev tcl-dev tk-dev \
libcairo2-dev mesa-common-dev libglu1-mesa-dev libncurses-dev

# Clone & Build Magic
git clone https://github.com/RTimothyEdwards/magic
cd magic
./configure
make
sudo make install


✅ Magic VLSI Successfully Installed

🎉 Installation Summary
Tool	Status	Primary Use
🧠 Yosys	✅ Complete	RTL Synthesis
📟 Iverilog	✅ Complete	Verilog Simulation
📊 GTKWave	✅ Complete	Waveform Analysis
⚡ Ngspice	✅ Complete	Circuit Simulation
🎨 Magic VLSI	✅ Complete	Layout Design
📂 Repository Info


