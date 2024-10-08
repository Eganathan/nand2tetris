# Notes on Nand2Tetris
References are available on the links.md file please do check it out

# Boolean Alegbra [video-link](https://youtu.be/Noi-lpSSEcE?list=PLrDd_kMiAuNmSb-CKWQqq9oBFN_KNMTaI)

## Basic

- AND (A ∧ B) => true if both are true. {1 AND 1 = 1, 1 AND 0 = 0}
- OR (A ∨ B) => True if at least one of A or B is true.{1 OR 0 = 1, 0 OR 0 = 0}
- NOT (¬A) => Inverts the value of A: True becomes False, and False becomes True.{NOT 1 = 0, NOT 0 = 1}
- NAND (A↑B) => True unless both A and B are true (the inverse of AND).{1 NAND 1 = 0, 1 NAND 0 = 1}
- NOR (A ↓ B) => True if neither A nor B is true (the inverse of OR).{0 NOR 0 = 1, 1 NOR 0 = 0}
- XOR (A ⊕ B) => True if A and B are different; False if they are the same (exclusive OR).{1 XOR 0 = 1, 1 XOR 1 = 0}
- XNOR (A ≡ B) => True if A and B are the same; False if they are different (inverse of XOR). {1 XNOR 1 = 1, 1 XNOR 0 = 0}

## The Truth Table

| A   | B   | NOT A | A AND B | A OR B | A XOR B | A NAND B | A NOR B | A XNOR B |
| --- | --- | ----- | ------- | ------ | ------- | -------- | ------- | -------- |
| 0   | 0   |   1   |    0    |    0   |    0    |    1     |    1    |    1     |
| 0   | 1   |   1   |    0    |    1   |    1    |    1     |    0    |    0     |
| 1   | 0   |   0   |    0    |    1   |    1    |    1     |    0    |    0     |
| 1   | 1   |   0   |    1    |    1   |    0    |    0     |    0    |    1     |

![alt text](https://introcs.cs.princeton.edu/java/71boolean/images/truth-table.png)

- NOT A: Inverts the value of A (0 becomes 1, and 1 becomes 0).
- A AND B: True only when both A and B are true (1).
- A OR B: True if either A or B (or both) are true.
- A XOR B: True if A and B are different (exclusive OR).
- A NAND B: The opposite of AND (true unless both A and B are true).
- A NOR B: The opposite of OR (true if neither A nor B is true).
- A XNOR B: True if A and B are the same (exclusive NOR).

# Axioms
![alt text](https://introcs.cs.princeton.edu/java/71boolean/images/axioms.png)
In addition, you can derive many other laws from these axioms. For example, the last entry in the table gives two special identities known as DeMorgan’s laws.
![alt text](https://introcs.cs.princeton.edu/java/71boolean/images/identities.png)
