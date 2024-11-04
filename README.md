# Low-Bit-Quantized-MAC

 <p align="center">
  <img width="800" height="500" src="low-bit quantised MAC.pdf">
</p>

[ View ](low-bit quantised MAC.pdf)


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
