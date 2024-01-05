---
title: "Verilog Vending Machine"
excerpt: "This is a vending machine implementation for FPGA boards in Verilog, which processes item selections and payments, calculates the total price, and displays the change due.<a href='https://youtu.be/U6rwh3BGOqA?si=hbOCRBfTlOrXEvY-'><br/><img src='/images/vending_machine.png'></a>"
permalink: /projects/vending-machine
collection: academic-projects
---

In our group project for Notre Dame's Logic Design and Sequential Circuits (CSE 20221) course, we created a vending machine simulation using Verilog, specifically tailored for the Altera DE2 board. The project features a prices module that calculates the total price of selected items based on input from switches, and this total price is then converted into binary-coded decimal format.

User inputs are managed through buttons, and a debounce mechanism ensures accurate and stable input capture. These inputs serve two functions: they help in setting the correct operational mode and reset values through a send reset and key to ROM module, and they are processed in the program calculator. This calculator, which forms the core of our system, adds specific amounts to a register or executes reset actions based on user input. The register accumulates the total sum of money inputted by the user.

The output from this register is then utilized in two key aspects: it is displayed on the LCD Message Table to show the total money inputted and the money owed, and it is used to calculate change using a greedy algorithm. This algorithm calculates the change in quarters, nickels, dimes, and pennies, which are then displayed on the DE2 board's HEX outputs.

Our system's functionality mirrors that of a vending machine. Users select items using switches and input money using buttons, with real-time display of the change due. The process concludes when the user presses a button to finalize the purchase and prepare the system for a new transaction.

To gain a better understanding of our project, the source code is available on [GitHub](https://github.com/johnflanagan827/Vending-Machine), or you can click on the image below to view a video tutorial.

<a href='https://youtu.be/U6rwh3BGOqA?si=hbOCRBfTlOrXEvY-'><br/><img src='/images/vending_machine.png'></a>