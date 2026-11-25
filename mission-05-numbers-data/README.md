# Mission 5 — Numbers, Python and text encoding

## 1. Task / objective

Convert decimal, binary and hexadecimal values by hand and with Python, build a number converter, and explain text encoding.

## 2. Work completed

### Task 5.1 — Manual conversions

| Question | Working | Answer |
|---|---|---|
| Decimal 13 to binary | 13 = 8 + 4 + 1 = `1101₂` | `1101₂` |
| Decimal 25 to binary | 25 = 16 + 8 + 1 = `11001₂` | `11001₂` |
| Binary 1010 to decimal | (1 × 8) + (0 × 4) + (1 × 2) + (0 × 1) | `10₁₀` |
| Binary 1101 to decimal | (1 × 8) + (1 × 4) + (0 × 2) + (1 × 1) | `13₁₀` |
| Hexadecimal A to decimal | A represents 10 in decimal. | `10₁₀` |
| Hexadecimal 1F to decimal | (1 × 16) + (15 × 1) | `31₁₀` |
| Binary 1111 to hexadecimal | One hexadecimal digit represents four binary bits: 1111 = F. | `F₁₆` |

### Task 5.2 — Python verification

| Expression tested | Result | Matches manual calculation |
|---|---|---|
| `bin(13)` | `'0b1101'` | Yes |
| `bin(25)` | `'0b11001'` | Yes |
| `int('1010', 2)` | `10` | Yes |
| `int('1101', 2)` | `13` | Yes |
| `hex(10)` | `'0xa'` | Yes |
| `hex(31)` | `'0x1f'` | Yes |
| `int('A', 16)` | `10` | Yes |
| `int('1F', 16)` | `31` | Yes |
| `format(int('1111', 2), 'X')` | `'F'` | Yes |

### Task 5.3 — Number converter

The converter is [number_converter.py](number_converter.py). It accepts a decimal integer, validates that it is positive, and prints `bin()` and `hex()` results.

| Test number | Binary output | Hexadecimal output |
|---|---|---|
| 13 | `0b1101` | `0xd` |
| 25 | `0b11001` | `0x19` |
| 42 | `0b101010` | `0x2a` |

`bin(number)` converts an integer to a binary string beginning with `0b`. `hex(number)` converts an integer to a hexadecimal string beginning with `0x`.

### Task 5.4 — Text encoding

- The ASCII decimal code for uppercase `A` is 65.
- The ASCII decimal code for lowercase `a` is 97.
- An encoding standard gives every character a consistent numeric representation so computers and software can store, transmit and recover text consistently.
- One character outside basic ASCII is `é`. UTF-8 can represent it and many other characters used across languages.

## 3. Commands / tools used

- `python3` — started Python for interactive checks and executed the converter.
- `bin()` — decimal to binary conversion.
- `int(value, base)` — conversion from binary or hexadecimal text to decimal.
- `hex()` — decimal to hexadecimal conversion.
- `format(number, 'X')` — hexadecimal-style formatting with uppercase letters.
- VS Code or a text editor — created source files.

## 4. My understanding

Bits are binary digits with values of zero or one, and eight bits make a byte. Number bases change how values are represented but do not change the underlying quantity. Character encodings define how letters and symbols become bytes.

## 5. Difficulties faced

No major difficulties.

## 6. How I resolved them

Not applicable.

## 7. Evidence / files

- [number_converter.py](number_converter.py)
- Manual calculations, Python verification and text encoding answers in this README

## 8. Commit details

- Meaningful commit message: `Build number converter and practise data representation`