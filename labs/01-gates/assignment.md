# Lab 1: Jakub Drápal

1. Equations of all three versions of logic function f(c,b,a):

   ![Logic function](pictures/logic.jpg)

2. Listing of VHDL architecture from design file (`design.vhd`) for all three functions. Always use syntax highlighting, meaningful comments, and follow VHDL guidelines:

    f_o      <= (not b_i and a_i) or (not c_i and not b_i);

    fnand_o  <= ((not b_i nand a_i) nand (not c_i nand not b_i));
    
    fnor_o   <= (b_i nor not a_i) or (c_i nor b_i);


3. Complete table with logic functions' values:

| **c** | **b** |**a** | **f(c,b,a)** | **f_NAND(c,b,a)** | **f_NOR(c,b,a)** |
| :-: | :-: | :-: | :-: | :-: | :-: |
| 0 | 0 | 0 | 1 | 1 | 1 |
| 0 | 0 | 1 | 1 | 1 | 1 |
| 0 | 1 | 0 | 0 | 0 | 0 |
| 0 | 1 | 1 | 0 | 0 | 0 |
| 1 | 0 | 0 | 0 | 0 | 0 |
| 1 | 0 | 1 | 1 | 1 | 1 |
| 1 | 1 | 0 | 0 | 0 | 0 |
| 1 | 1 | 1 | 0 | 0 | 0 |

### Distributive laws

1. Screenshot with simulated time waveforms. Always display all inputs and outputs (display the inputs at the top of the image, the outputs below them) at the appropriate time scale!

   ![Logic function](pictures/wave.png)

2. Link to your public EDA Playground example:

   https://www.edaplayground.com/x/fBkq
