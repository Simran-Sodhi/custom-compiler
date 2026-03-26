# Compiler Construction

A compiler front-end implemented in C for a custom programming language, supporting lexical analysis, grammar-based parsing, token generation, and syntax validation.

This project was developed as part of a compiler construction course and focuses on building core components of a language-processing pipeline from scratch.

---

## Features

- Lexical analysis for tokenizing source code
- Comment removal utility
- Token list generation with line numbers
- Grammar-based parsing using FIRST and FOLLOW sets
- Predictive parsing using parse table construction
- Syntax checking for input source programs
- CPU time measurement for lexer and parser execution

---

## Project Structure

- `driver.c` – Menu-driven entry point for running compiler functionalities  
- `lexer.c`, `lexer.h`, `lexerDef.h` – Lexical analyzer implementation  
- `parser.c`, `parser.h`, `parserDef.h` – Parser implementation  
- `Grammar.txt` – Grammar specification  
- `First.txt` – FIRST sets  
- `Follow.txt` – FOLLOW sets  
- `NTerminals.txt` – Non-terminal definitions  
- `tokenId.txt` – Token mapping/reference  
- `t1.txt` to `t6.txt` – Sample test cases  
- `makefile` – Build instructions  

---

## Build

Compile the project using:

    make

This generates the executable:

    stage1exe

---

## Run

Run the compiler front-end with:

    ./stage1exe <input_file> <output_file>

Example:

    ./stage1exe t1.txt output.txt

---

## Menu Options

After running the executable, choose from:

- `0` – Exit  
- `1` – Remove comments and print cleaned code  
- `2` – Print token list  
- `3` – Check syntactic correctness of the input source code  
- `4` – Print total time taken by lexer and parser  

---

## Concepts Implemented

- DFA-based lexical analysis  
- Token recognition and symbol handling  
- Grammar representation  
- FIRST and FOLLOW set computation  
- Predictive (LL) parsing  
- Parse table construction  
- Syntax validation  

---

## Sample Output

The program can:

- Print lexemes and token names with line numbers  
- Validate syntactic correctness of input programs  
- Generate parser-related output files  

---

## Notes

- This project focuses on compiler front-end design (lexing + parsing), not code generation  
- Grammar and parsing data are loaded from external text files  
- Sample test inputs are included in the repository  

---

## Acknowledgment

Developed collaboratively as part of a compiler construction course at BITS Pilani.
