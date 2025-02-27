# Half Adder
The purpose of this repository is to show my understanding of binary addition and how it applies in theory and in practice. To do this I will explain one of the simplest ways to add two binary numbers together: the half adder. A half adder is a circuit meant to compute the first digit of binary addition. This circuit forms the foundation of more complicated circuits like the full and 4-bit adder.

As a short recap: binary numbers are comprised of only 0's and 1's. This is different than decimal numbers, which are comprised of any digits 0-9. The limited number of digits means that binary numbers grow larger faster than decimal. So 0, 1, 2, 3, 4, 5 in decimal is 0, 1, 10, 11, 100, 101 in binary.
![halfadderdiagram1](https://github.com/user-attachments/assets/4a7bd939-690d-4ba2-95c2-e6c7ca9ef273)
In the diagram, the half adder (HA) takes two inputs, A and B, as the two binary digits to add. The Sum is outputted through S, and Cout is the digit to Carry to the next place value. The half adder itself is made with two logic gates: a XOR and an AND gate. The XOR gate handles the sum, while the AND gate determines the carry value.
![halfaddergates2](https://github.com/user-attachments/assets/bb4448d2-652d-4155-ad9c-e6d535ed034a)
Since a half adder is made with logic gates and has a limited number of inputs, we can visualize every possible output it could have with the truth table shown below. With this, we can confirm a number of solutions. For example, 0 + 0 will be equal to 0, and 1 + 1 will return a Sum of 0 with a Carry of 1.

![image](https://github.com/user-attachments/assets/3bae16b7-ad69-4fd4-9ac8-9336dfa24690)

With all of this information in mind, we can now recreate a half adder using integrated circuits. The integrated circuits I'll be using are simply multiple logic gates packed onto one chip. I'll use the circuit diagram below to construct a simple half adder circuit.

![image](https://github.com/user-attachments/assets/676e41c9-2896-42b4-a1df-dcea67bafca5)
![image](https://github.com/user-attachments/assets/b82dd687-b5b0-4831-baa6-a484df6a08a2)

In the above image, the half adder is adding two binary zeros together. This explains why both the S and Cout LEDs are off; 0 + 0 returns a Sum of 0 and a Carry value of 0. If we wanted to change the bits we're adding together, we just have to flip the first or last switch. Below, I flip switch B on so that I'm adding 0 and 1 together.
![image](https://github.com/user-attachments/assets/394338a6-7c7c-4a67-9b35-46504634376a)

This combination illuminates the S LED because 0 + 1 equals 1. Both of these examples make sense, but something interesting happens when we flip both inputs on.
![image](https://github.com/user-attachments/assets/eb288120-17ed-48d5-908d-d2276f663766)

