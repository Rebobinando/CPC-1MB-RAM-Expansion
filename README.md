# CPC 1MB RAM Expansion

## What is this? Why?

Based on the original design from Revaldinho Amstrad CPC RAM Expansion, this design propose a smaller board form factor. This version then, fits into the many expansion boards available up to now.

This allows, as well as the original design, to enjoy 1MB RAM in our CPC. Other sizing as 64Kb or 512Kb extra RAM configuration are achievable through the 4 switches on the top of the board. This development, as well as Revaldinho design, works on a CPC464, CPC664 and CPC6128.

Original design and complete description are available at [Revaldinho Github](https://github.com/revaldinho/cpc_ram_expansion/tree/master/cpc_ram_expansion1mb)

More development details are available in [VadeRetro forum](https://www.va-de-retro.com/foros/viewtopic.php?t=10455)

## Features

Some differences from the original design:

- There is an added voltage regulator added to allow the supply of 3.3V to the CPLD.
- Some capacitors (3x100NF and 2x10uF) and the voltage regulator are SMD form factor to allow smaller size to board.
- CPLD XC9572XL is adopted and preferred because of its better availability in the market compared to XC9572.
- There is a jumper that allows the selection of which voltage we want to supply to the CPLD:
	  * 5V allows to use XC9572 and XC9536.
	  * 3.3V allows to use XC9572XL and XC9536XL.
- 4-Switch 90 degrees are adopted to allow better accessibility once connected to the expansion board.

CPLD programming is fully compatible with original version available at Revaldinho Gitub. Additional non existing versions in Revaldinho Github are available here.

## Bill of materials

|Qty| Component     | Value               |  Package  |
|---|---------------|---------------------|-----------|
| 2 | Capacitor     | 10uF                | SMD C0805 | 
| 3 | Capacitor     | 100nF               | SMD C0805 |
| 1 | Capacitor     | 22pF - 25V Elec     | DIP  4x1.5|
| 1 | Voltage Reg   | AMS1117-3.3         | SOT223    |
| 1 | CPLD          | XC9572XL            | PLCC44    |
| 2 | RAM           | 628512              | DIP       |
| 1 | pin           | 1x7                 | DIP       |
| 1 | pin           | 1x3                 | DIP       |
| 2 | Resistor net  | 5PIN 3.3K           | DIP       |
| 1 | Switch        | 4 bit               | DIP       |
| 1 | MX4 connector | DC3-50P Right Angle | DIP       |
| 2 | Socket        | 32p - Wide          | DIP       |
| 1 | Socket        | PLCC44              | DIP       |

## Board layout

These are the main elements in the top face:

![Top](https://github.com/Rebobinando/CPC-1MB-RAM-Expansion/blob/main/Pic/Top%20Details.PNG)

In the bottom face, we will find the SMD components:

![Bottom](https://github.com/Rebobinando/CPC-1MB-RAM-Expansion/blob/main/Pic/Bottom%20Details.PNG)

And this is the board installed onto the CPC expansion board:

![RAM Expansion](https://github.com/Rebobinando/CPC-1MB-RAM-Expansion/blob/main/Pic/CPC%20RAM%20Expansion%20MX4_Inserted.jpg)

## Warning & Disclaimer
If you want to build yourself, please proceed and read carefully all this information. Bear in mind that all the information in this project is published in good faith and for general information purpose only. I do not make any warranties about the completeness, reliability, and accuracy of this information. Any action you take upon the information you find here, is strictly at your own risk. I will not be liable for any losses and/or damages. 

## Thanks to

- Revaldinho for publishing all his original design information, making it accessible for the whole users community.

- All the users for VadeRetro forum, who supported the initial batch of units.


## Redistribution

All programs and data files in this project are made available under the terms of the [GNU General Public License v3](https://github.com/Rebobinando/CPC-1MB-RAM-Expansion/blob/main/LICENSE)
