# Mission 5 — Numbers and data

## 1. Task / objective
Convert decimal, binary and hexadecimal values, verify them with Python, build a small number converter and explain how text is encoded.

## 2. Work completed

### Task 5.1: Manual conversions

| Question | Your working and answer |
|---|---|
| Decimal 13 to binary | 13÷2=6 r1, 6÷2=3 r0, 3÷2=1 r1, 1÷2=0 r1. Reading remainders from bottom to top: 1101 |
| Decimal 25 to binary | 25÷2=12 r1, 12÷2=6 r0, 6÷2=3 r0, 3÷2=1 r1, 1÷2=0 r1. Reading bottom to top: 11001 |
| Binary 1010 to decimal | 8+0+2+0 = 10 |
| Binary 1101 to decimal | 8+4+0+1 = 13 |
| Hexadecimal A to decimal | A = 10 |
| Hexadecimal 1F to decimal | 1×16 + 15 = 31 |
| Binary 1111 to hexadecimal | 1111 is one group of four bits = 8+4+2+1 = 15 = F |

### Task 5.2: Python verification

| Expression tested | Result | Matches my manual answer? |
|---|---|---|
| bin(13) | 0b1101 | Yes |
| bin(25) | 0b11001 | Yes |
| int("1010", 2) | 10 | Yes |
| int("1101", 2) | 13 | Yes |
| int("A", 16) | 10 | Yes |
| int("1F", 16) | 31 | Yes |
| hex(15) | 0xf | Yes (F) |

The `0b` and `0x` at the start of the results only show that the number is in binary or hexadecimal.

### Task 5.3: Number converter
I created `number_converter.py`. It asks the user to enter a decimal number, converts the input to an integer, and prints the binary and hexadecimal forms.

- `input()` reads what the user types as text.
- `int()` converts that text into a whole number.
- `bin()` returns the binary form of a number.
- `hex()` returns the hexadecimal form of a number.

| Test number | Binary output | Hexadecimal output |
|---|---|---|
| 10 | 0b1010 | 0xa |
| 25 | 0b11001 | 0x19 |
| 255 | 0b11111111 | 0xff |

### Task 5.4: How text is stored
- The ASCII code for uppercase A is 65 and for lowercase a is 97 (found with `ord()`).
- Computers only store numbers, so an encoding standard is needed to decide which number stands for which character. This lets every device read the same text correctly.
- An example of a character that is not in basic ASCII is ₹ (the rupee sign).

## 3. Commands / tools used
- `python3` – opened the Python interactive environment
- `bin()`, `hex()`, `int()`, `ord()` – Python functions for conversion and character codes
- `input()` – reads user input in the converter
- `python3 number_converter.py` – ran the converter
- Tools: VS Code, zsh terminal
