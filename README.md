## Exp-No: 02 - Write and simulate seven segment display using Verilog HDL and verify with testbench
# Aim:

  To design and simulate a Seven Segment using Verilog HDL and verify its functionality through a testbench using the Vivado 2023.1 simulation environment.
  
# Apparatus Required:

  Vivado 2023.1

# Procedure:

- Launch Vivado Open Vivado 2023.1 by double-clicking the Vivado icon or searching for it in the Start menu.  

- Create a New Project Click on "Create Project" from the Vivado Quick Start window. In the New Project Wizard:  
  - Project Name: Enter a name for the project (e.g., Seven_Segment_Display).  
  - Project Location: Select the folder where the project will be saved.  
  - Click Next.  
  - Project Type: Select RTL Project, then click Next.  
  - Add Sources: Click on "Add Files" to add the Verilog file (e.g., seven_segment.v) and the testbench file (seven_segment_tb.v). Make sure to check the box "Copy sources into project" to avoid external file dependencies. Click Next.  
  - Add Constraints: Skip this step by clicking Next (since no constraints are needed for simulation).  
  - Default Part Selection: Choose a part based on the FPGA board being used. If no board is used, choose any part such as xc7a35ticsg324-1L (Artix-7). Click Next, then Finish.  

- Add Verilog Source Files In the "Sources" window, right-click on "Design Sources" and select Add Sources if you did not add all files earlier. Add the Verilog design file (seven_segment.v) and testbench file (seven_segment_tb.v).  

- Check Syntax Expand the "Flow Navigator" on the left side of the Vivado interface. Under "Synthesis", click "Run Synthesis". Vivado will check the design for syntax errors. If any errors or warnings appear, correct them in the respective Verilog files and re-run the synthesis.  

- Simulate the Design In the Flow Navigator, under "Simulation", click on "Run Simulation" → "Run Behavioral Simulation". Vivado will open the Simulations Window, and the waveform window will show the signals defined in the testbench.  

- View and Analyze Simulation Results Verify the segment outputs (a–g) for each input digit (0–9) and confirm that they match the expected seven-segment display pattern.  

- Adjust Simulation Time To run a longer simulation or adjust timing, go to the Simulation Settings by clicking "Simulation" → "Simulation Settings". Under "Simulation", modify the Run Time (e.g., set to 1000ns).  

- Generate Simulation Report Once the simulation is complete, generate a simulation report by right-clicking on the simulation results window and selecting "Export Simulation Results". Save the report for future reference.  

- Save and Document Results Save the project by clicking File → Save Project. Take screenshots of the waveform window and include them in the lab report to document the correct operation of the seven-segment display for all input combinations.  

- Close the Simulation Once done, go to Simulation → "Close Simulation".  



# RTL Code:

<img width="1917" height="1078" alt="hdl_1_2" src="https://github.com/user-attachments/assets/2b2e0632-ec8e-4480-abf7-75896e975e52" />


# TestBench:

<img width="1862" height="1077" alt="hdl_1_4" src="https://github.com/user-attachments/assets/898d6fc1-bfc0-40c1-8ace-82a5e9f1704a" />


# Output waveform:

<img width="1917" height="1077" alt="hdl_1_1" src="https://github.com/user-attachments/assets/284e77b0-9a48-4bb2-8ffc-6ba9dd32f2e3" />

<img width="1918" height="1078" alt="hdl_1_3" src="https://github.com/user-attachments/assets/0ff6e8fd-4c7b-4bbd-accb-6ce34c85d83a" />


# Conclusion:


In this experiment, a seven-segment display decoder was designed and simulated using Vivado 2023.1. The Verilog code was implemented to convert binary-coded decimal (BCD) inputs into appropriate segment control signals. The behavioral simulation verified that each digit (0–9) was correctly displayed by activating the corresponding segments (a–g).  

Thus, the experiment successfully demonstrated the design and working of a seven-segment display using Verilog HDL and provided practical experience with synthesis and simulation in Vivado



