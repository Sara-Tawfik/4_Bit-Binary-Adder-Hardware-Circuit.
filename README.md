# 4-Bit Binary Full Adder Hardware Circuit 🔌➕

## 📌 Project Overview
A physical and simulated digital logic circuit designed to perform binary addition of two 4-bit numbers (ranging from 0 to 15 decimal). The system takes inputs via two 4-bit switches, processes the dynamic mathematical addition using a **Full Adder Integrated Circuit (IC)**, and displays the final sum as a 5-bit binary output via a bank of illuminated **LEDs**.

The layout safely accounts for the 5th bit output by capturing it through the **Carry-Out (Cout)** function of the adder circuit.

Developed as part of the **CSAI 102 Digital Logic and Computer Architecture** course at the University of Science and Technology in zewailcity.

---

## 🛠️ Circuit Design & Architecture
The design implementation is divided into three major blocks mapping inputs directly to a hardware system:

1. **Input Configuration**: Two independent 4-bit switches provide the binary inputs. Resistors are strategically added to pull down the switch inputs to the ground, successfully **preventing floating point random inputs** when no switch lines are triggered.
2. **Processing Unit**: Uses a **Full Adder IC**.The pin assignments route individual bits from Switch 1 ($Input_0$ to $Input_3$) and Switch 2 ($Input_0$ to $Input_3$) directly into the IC's addition pins. The Initial Carry-In ($C_{in}$) is securely grounded to zero.
3. **Output Interface**: The summation output pins ($S_0$ to $S_3$) along with the final Carry-Out ($C_{out}$) pin drive 5 independent LEDs. Resistors protect each LED's cathode to ground.

---

## 💻 Simulation Setup
* **Software**: Logisim.
* **File Included**: `4bit_adder_design.circ` (Open via Logisim to test binary configurations and watch the LEDs change dynamically).
* *Note on Simulation*: Logisim handles the 5th bit output natively through the carry flag ($C_{out}$) to display sums up to 30.

---

## 👥 Team Members
* **Sara Taha Tawfik** 
* **Menna Mohammed Hassan** 

**Supervised by**: Dr. El Mahdy Maree & Eng. 
