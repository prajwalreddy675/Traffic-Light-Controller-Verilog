# Traffic Light Controller Using Verilog

## 1. Project Overview
This project implements a Traffic Light Controller using Verilog HDL and a Finite State Machine (FSM).

It controls traffic signals for two directions:
- North-South (NS)
- East-West (EW)

## 2. Objective
To design and simulate a four-state traffic light controller using Verilog.

## 3. Tools Used
- Visual Studio Code
- Ubuntu (WSL)
- Icarus Verilog
- GTKWave
- Yosys

## 4. Working Principle
The controller uses four states:

| State | North-South | East-West |
|---|---|---|
| State 0 | Green | Red |
| State 1 | Yellow | Red |
| State 2 | Red | Green |
| State 3 | Red | Yellow |

The controller changes states with each clock cycle. Reset initializes the controller to State 0.

## 5. Output Encoding
- 00 = Red
- 01 = Yellow
- 10 = Green

## 6. Project Files
- `traffic_light_controller.v` – Main Verilog design.
- `tb_traffic_light.v` – Testbench.
- `traffic_light_tb.vcd` – Simulation waveform data.
- `traffic_circuit.png` – Generated circuit diagram.
- `traffic_circuit.dot` – Circuit diagram source.
- `traffic_tb` – Comp