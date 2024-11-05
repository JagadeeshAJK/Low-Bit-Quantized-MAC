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








This project focuses on the design and analysis of a low-bit quantized Multiply-Accumulate (MAC) circuit. It explores the impact of quantization on data representation and performance, comparing both 16-bit and 4-bit data.

## Product Calculation and Quantization Analysis

### For 16-Bit Data:
- **Max Product Value**: 
  - 65535 * 65535 = 4.3 x 10^9
- **Example Values**:
  - **A**: 55555 (Binary: `1101_1001_0000_0011`)
  - **B**: 23603 (Binary: `0101_1100_0011_0011`)
- **Product**:
  - A * B = 55555 * 23603 = 1311264665
- **Percentage of Max**:
  - (1311264665 / (4.3 x 10^9)) ≈ 30.4% (approximately 30%)

### For 4-Bit Data:
- **Max Product Value**:
  - 15 * 15 = 225

- **Quantized Values**:
  - **A**: `1101` (Quantized value = 13)
  - **B**: `0101` (Quantized value = 5)

- **Product**:
  - 13 * 5 = 65

- **Percentage of Max**:
  - (65 / 225) ≈ 28.9% (approximately 29%)

















9007     **0010**001100101111  3     9%<br>
44272    **1010**110011110000  10       13.3%


## Future work 
1. **Exploration of Alternative Quantization Schemes:** Research alternative quantization methods, such as stochastic quantization or adaptive quantization, to see if they offer improvements over the current approach.<br>
2. **Design Modifications:** Implement design modifications, like using different types of adders (e.g., carry-lookahead or carry-save) to improve speed and efficiency.<br>
3. **Improving Accuracy:** Experiment with different quantization techniques or bit-widths to find the best trade-off between performance and accuracy.<br>
4. **Dynamic Quantization Techniques:** Explore advanced dynamic quantization methods to adaptively adjust the quantization levels based on input data statistics. This could improve the accuracy of the MAC operation.<br>
5. **Adaptive Quantization:** Implement an adaptive quantization scheme that adjusts the quantization levels based on input signal characteristics to improve efficiency and accuracy.<br>

## Contributors
- Kunal Ghosh
## Acknowledgments
Kunal Ghosh, Director, VSD Corp. Pvt. Ltd.
## Contact Information
Kunal Ghosh, Director, VSD Corp. Pvt. Ltd. kunalghosh@gmail.com
## References:
1. https://chatgpt.com/
2.	https://youtu.be/VCuyO7Chvc8?si=j08shJ8WrL5gbNtt
3.	https://images.app.goo.gl/42Hqv37epNisBSMo7



