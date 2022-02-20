# Lab 2: Jakub Drápal

### 2-bit comparator

1. Karnaugh maps for other two functions:

   Greater than:

   ![greater.jpg](greater.jpg)

   Less than:

   ![less.jpg](less.jpg)

2. Equations of simplified SoP (Sum of the Products) form of the "greater than" function and simplified PoS (Product of the Sums) form of the "less than" function.

   ![functions.jpg](functions.jpg)

### 4-bit comparator

1. Listing of VHDL stimulus process from testbench file (`testbench.vhd`) with at least one assert (use BCD codes of your student ID digits as input combinations). Always use syntax highlighting, meaningful comments, and follow VHDL guidelines:

   My student ID: **229322**

```vhdl
    p_stimulus : process
    begin
        -- Report a note at the beginning of stimulus process
        report "Stimulus process started" severity note;

        -- Test values
        s_b <= "0010"; s_a <= "0010"; wait for 100 ns;
        assert ((s_B_greater_A = '0') and (s_B_equals_A = '1') and (s_B_less_A = '0'))
      
        report "Test failed for input combination: 0010, 0010" severity error;
        report "Stimulus process finished" severity note;
        wait;
    end process p_stimulus;
```

2. Text console screenshot during your simulation, including reports.

   ![screen.png](screen.png)

3. Link to your public EDA Playground example:

   [https://www.edaplayground.com/x/StKN](https://www.edaplayground.com/x/StKN)
