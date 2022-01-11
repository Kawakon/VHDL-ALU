# Four Operation Arithmetic Logic Unit using VHDL

In this project, a four operation arithmetic logic unit (ALU) is design in VHDL. The ALU is designed on a Intel IV E EP4CE115F29C7 FPGA. The operations that can 
be performed by the ALU are addition, logic OR, multiplication, and division. The ALU performs these operations
on 8-bit operands and the results are printed onto a seven-segment LED display in hexadecimal. The 8-bit binary
result is also displayed by a sequence of LEDs. A diagram of the ALU can be seen below:

![image](https://user-images.githubusercontent.com/43174428/148951311-1af394ef-b0ab-4094-9b3f-3e753d594224.png)

## Hardware

The hardware for the ALU includes registers, a 4-1 multiplexer, seven-segment decoders, seven-segment LEDs, and LEDs. The VHD files for these components can be found in this project. 

## Operations

The operands A and B are provided to the ALU using the switches on the FPGA and the ENABLE_1 signal. The addition operation simply adds the values of A and B. The logic OR operation performs a logical OR on A and B and returns the result. The division operation  divides the operand A by 2. This is done by shifting the value of A one bit to the right within a shift register. The multiplication operation multiplies the operand A by 2. This is performed by shifting the value of A one bit to the left within a shift register. 

