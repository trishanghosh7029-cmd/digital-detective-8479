# Mission 4 — How programs run

## 1. Task / objective

Create and execute a simple Python program, then compare compilers and interpreters.

## 2. Work completed

Created [hello.py](hello.py), which prints `Hello from Python`. It was run with Python 3 and confirmed to display the required message.

### Compiler and interpreter comparison

| Point | Compiler | Interpreter |
|---|---|---|
| When translation / execution happens | Translates source code before execution, then runs the resulting form. | Reads and executes source instructions during the run. |
| Typical output | Usually a separate executable or intermediate build output. | The program's ordinary output, with no required separate executable. |
| One example | A C compiler producing machine-code output. | Python executing source code through an interpreter. |
| One advantage | Compiled output can often be optimized and later run without recompiling. | Changes can be tested quickly without a separate compilation step. |

A compiler translates complete source code into another form before the program is run. An interpreter carries out instructions while reading the program, usually at runtime. Real implementations can combine both approaches: Python source is commonly compiled to bytecode before bytecode is executed by a virtual machine.

## 3. Commands / tools used

- `python3 hello.py` — executes the Python source file.
- Python 3 — provides the interpreter used for this mission.
- VS Code or a text editor — created and reviewed `hello.py`.

## 4. My understanding

Source code is instructions written in a programming language. An interpreter performs those instructions at runtime, while a compiler performs a translation stage before normal execution. Both approaches provide a way for software to run on a computer.

## 5. Difficulties faced

No major difficulties.

## 6. How I resolved them

Not applicable.

## 7. Evidence / files

- [hello.py](hello.py)
- This README contains the compiler/interpreter comparison.

## 8. Commit details

- Meaningful commit message: `Compare compilers and interpreters`