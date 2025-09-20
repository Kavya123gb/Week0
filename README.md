# 🚀 **Week 0: VLSI System Design (VSD) Program Foundation & Tool Setup**

## 📌 **VLSI Week 0 Status**

Welcome to my **VLSI System Design (VSD) Program repository**!  
This week focused on setting up the development environment and installing the **essential open-source tools** that will be used throughout the program.  
The goal was to create a **reliable and efficient workspace** for synthesis, simulation, and design tasks.  

---

## 🎯 **System and Virtual Machine Configuration**

To ensure optimal performance, I configured a **Virtual Machine (VM)** with the following specifications:  

| Specification 💻 | Details 📋 |
|------------------|------------|
| **Operating System 🐧** | Ubuntu 20.04+ |
| **RAM 💾** | 6GB |
| **Storage 💿** | 50GB HDD |
| **vCPUs ⚡** | 4 |

💡 **Pro Tip:** This setup guarantees sufficient resources for handling toolchain demands and running simulations smoothly.  

---

## ⚙️ **Tool Installation & Verification**

The following tools were installed for **RTL synthesis, simulation, circuit analysis, and layout design**.  
Below are the installation steps and verification commands.  

🧠 Yosys → 📟 Iverilog → 📊 GTKWave → ⚡ Ngspice → 🎨 Magic VLSI  

---

### 🧠 **1. Yosys – RTL Synthesis Tool**  
**Purpose:** Converts RTL code into gate-level representations.  

```bash
# Day 0 - Tools Installation
## Yosys
git clone https://github.com/YosysHQ/yosys.git
cd yosys 

# Dependencies
sudo apt install make
sudo apt-get install build-essential clang bison flex \
libreadline-dev gawk tcl-dev libffi-dev git \
graphviz xdot pkg-config python3 \
libboost-system-dev libboost-python-dev \
libboost-filesystem-dev zlib1g-dev

# Build & Install
make 
sudo make install

sudo apt-get install iverilog

sudo apt update
sudo apt install gtkwave

sudo apt update
sudo apt install ngspice

# Install dependencies
sudo apt-get install m4 tcsh csh libx11-dev tcl-dev tk-dev \
libcairo2-dev mesa-common-dev libglu1-mesa-dev libncurses-dev

# Clone repository
git clone https://github.com/RTimothyEdwards/magic
cd magic

# Configure & Build
./configure
make

# Install
sudo make install

| Tool              | Status     | Primary Use        |
| ----------------- | ---------- | ------------------ |
| 🧠 **Yosys**      | ✅ Complete | RTL Synthesis      |
| 📟 **Iverilog**   | ✅ Complete | Verilog Simulation |
| 📊 **GTKWave**    | ✅ Complete | Waveform Analysis  |
| ⚡ **Ngspice**     | ✅ Complete | Circuit Simulation |
| 🎨 **Magic VLSI** | ✅ Complete | Layout Design      |
