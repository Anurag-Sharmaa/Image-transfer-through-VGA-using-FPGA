Image Transfer Through VGA Using FPGA
This project demonstrates image display using an FPGA board and a VGA interface. Specifically, it involves displaying two versions of an image (an original and an inverted version) on a monitor using VGA signals generated directly through Verilog code, without using any BRAM IP cores.

Project Overview
Images Used: Two images are used for demonstration:

A base image (e.g., a photo of "Ben.txt").

An inverted version of the same image (pixel inversion performed externally).: Inverted_Ben.txt

Conversion: These images are pre-processed and converted into .txt files containing pixel data.

Storage: The .txt files are stored under the directory:
projectname.srcs/sources_1/new/
Implementation: The design is implemented in Verilog and can be simulated and synthesized using the Xilinx Vivado Design Suite.

Hardware Platform
The code is intended to run on the Nexys 4 DDR and Basys 3 FPGA board.

The necessary .xdc constraint files are provided for both the Basys 3 and Nexys 4 DDR boards in the repository.

Note: Ensure you follow the Nexys 4 DDR Reference Manual for VGA connections and hardware setup.

Entire image storage and handling is done manually using Verilog constructs.

Tested on real hardware using the Nexys 4 DDR board.

Getting Started
Place your .txt image files in projectname.srcs/sources_1/new/.

Open the project in Vivado.

Use the appropriate .xdc file for your board (Basys 3 or Nexys 4 DDR).

Synthesize, implement, and generate the bitstream.

Connect the board to a monitor using a VGA cable.

Program the FPGA and observe the image display.

Resources Used
YouTube Tutorial: https://youtu.be/UqdIBD4pJIU?si=utRE0ZroyMQfkUeE

Nexys 4 DDR Reference Manual: https://digilent.com/reference/_media/reference/programmable-logic/nexys-4-ddr/nexys4ddr_rm.pdf

