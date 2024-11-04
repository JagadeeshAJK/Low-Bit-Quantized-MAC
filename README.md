# Low-Bit-Quantized-MAC
This Project simulates Low-Bit Quantized MAC (Multiply-Accumulate) reduces data precision to save memory and computation, making it efficient for low-power applications.
[ View ](https://github.com/JagadeeshAJK/Low-Bit-Quantized-MAC/blob/main/low-bit%20quantised%20MAC.pdf)



# Introduction to Low-Bit Quantized MAC

A low-bit quantized Multiply-Accumulate (MAC) circuit processes reduced-precision data, typically by lowering the bit-width of operands (e.g., from 16-bit to 4-bit). This quantization reduces memory usage and computation requirements, making it especially useful in energy-efficient hardware, such as AI accelerators and edge devices, where minimizing power consumption is crucial. However, low-bit quantization can impact accuracy, so careful design is essential to balance performance and efficiency.



# circuit diagram for Low-Bit-Quantized-MAC
 ![pro](https://github.com/JagadeeshAJK/Low-Bit-Quantized-MAC/blob/main/project.png)

### Building Blocks of the Circuit 
- **Logic Gates**
  - **XOR Gate**:
  - **AND Gate**:
  - **OR Gate**:
- Schematic: ![XOR Gate Schematic](path/to/xor_gate_schematic.png)
- **Arithmetic Components**
  - **Adder**: 
  - **Multiplier**: Description...
- Schematic: ![Adder Schematic](path/to/adder_schematic.png)


# Mapping of Quantization Levels
| Original Range | Quantized Value |
|----------------|-----------------|
| 0-4095         | 0               |
| 4096-8191      | 1               |
| 8192-12287     | 2               |
| 12288-16383    | 3               |
| 16384-20479    | 4               |
| 20480-24575    | 5               |
| 24576-28671    | 6               |
| 28672-32767    | 7               |
| 32768-36863    | 8               |
| 36864-40959    | 9               |
| 40960-45055    | 10              |
| 45056-49151    | 11              |
| 49152-53247    | 12              |
| 53248-57343    | 13              |
| 57344-61439    | 14              |
| 61440-65535    | 15              |




# Low Bit Quantized MAC

## Overview
This project focuses on the design and analysis of a low-bit quantized Multiply-Accumulate (MAC) circuit. It explores the impact of quantization on data representation and performance, comparing both 16-bit and 4-bit data.

## Product Calculation and Quantization Analysis

### For 16-Bit Data:
- **Max Product Value**: 
  \[
  65535 \times 65535 = 4.3 \times 10^9
  \]
- **Example Values**: 
  - **A** = 55555
  - **B** = 23603
- **Product**: 
  \[
  A \times B = 1311264665
  \]
- **Percentage of Max**: 
  \[
  \frac{1311264665}{4.3 \times 10^9} \approx 30.4\% \quad (\text{approximately } 30\%)
  \]

### For 4-Bit Data:
- **Max Product Value**: 
  \[
  15 \times 15 = 225
  \]
- **Quantized Values**: 
  - **A**: `1101100100000011` (Quantized value = **13**)
  - **B**: `0101110000110011` (Quantized value = **5**)
- **Product**: 
  \[
  13 \times 5 = 65
  \]
- **Percentage of Max**: 
  \[
  \frac{65}{225} \approx 28.8\% \quad (\text{approximately } 29\%)
  \]

## Highlighting the Last Four Significant Bits
In the context of the 4-bit quantized data:
- The last four significant bits of **A**:
- 














For 16 bit data max product value is 665535*65535=4.3x10^9<br>
For 4 bit data max product value is 15*15=225<br>

If data is A=55555 and B=23603 the product is 1311264665<br>
A*B value of 16 bit data is 30.4% =30% of the max of 16 bit product <br>

The Quantized value for A   **1101**100100000011 is 13<br>
The Quantized value for B   **0101**110000110011 is 5<br>
The product is 13*5 =65<br>
A*B value of 4 bit data is 28.8% = 29% of the max of 4 bit product<br>

<span style="background-color: yellow; color: black;">0011</span>100


9007     **0010**001100101111  3     9%<br>
44272    **1010**110011110000  10       13.3%
