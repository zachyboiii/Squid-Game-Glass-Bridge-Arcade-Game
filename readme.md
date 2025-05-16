# Glass Bridge Arcade Game 🎮

Inspired by Netflix’s *Squid Game*, this project is an FPGA-based arcade game where players must cross a virtual glass bridge by correctly guessing the safe path—left or right—at each step. The game integrates core concepts from digital logic and CPU architecture, including FSMs, ALUs, register files, and a custom datapath. It is fully implemented using **Lucid HDL**, a hardware description language used with the Alchitry Labs toolchain.

## 🔧 Project Overview

Players begin by pressing the **Start** button and selecting a difficulty level:

- 🟠 **Easy**: 60 seconds
- 🟦 **Medium**: 30 seconds
- 🔺 **Hard**: 15 seconds

A randomly generated path determines the correct choices. Each correct guess advances the player, while a wrong guess resets progress to the beginning. The goal is to reach the end of the bridge before the timer runs out.

## 💡 Features

- ✅ Implemented entirely in **Lucid HDL**
- ✅ Difficulty selection via buttons
- ✅ Random bridge path generation
- ✅ Seven-segment display for countdown timer
- ✅ Bicolored LEDs for visual bridge path representation
- ✅ Finite State Machine (FSM) controlling game states
- ✅ Custom datapath with ALU and register file (inspired by Beta CPU)
- ✅ Reset and restart functionality

## 🧠 Technical Concepts

- **Lucid HDL:** Hardware description language used for all module definitions and logic
- **FSM (Finite State Machine):** Controls game flow and transitions
- **ALU (Arithmetic Logic Unit):** Evaluates player input and timer logic
- **Register File:** Stores and updates game state values (e.g., step count, timer)
- **Datapath Design:** Mimics Beta CPU-style instruction/data flow
- **Debounced Inputs:** Reliable button press detection
- **Random Logic:** Generates new bridge paths on each game reset

## 🖥️ Hardware Requirements

- FPGA Development Board (e.g., Alchitry Au / Mojo / DE0-Nano)
- Bicolored LEDs
- Seven-segment display
- Push buttons (Start, Circle, Square, Triangle)
