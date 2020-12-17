# ESP32_Bat_Pro
The repository contains the file for the ESP32_Bat_Pro board, an enhanced version of the ESP32_Bat board.
The LC709203F.zip file contains the driver library for the State of Charge monitor IC.

The ESP32_Bat and ESP32_Feather boards do not have a good way of monitoring the state of charge of the LiPo cell.  The LC709203F SOC IC is an excellent monitor of the state of charge of the LiPo cell.  It does not perform coulomb counting so the errors do not accumulate over time.  It compensates for the aging of the cell and accurately tracks the capacity of the cell while the cell is charging or discharging.  The LC709203F can measure the cell voltage accurately without the need for a resistor divider network.  It can also generate an interrupt to the ESP32 if the cell capacity falls below a given percentage or the if the cell voltage falls below a setpoint.
