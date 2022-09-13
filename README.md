<p align="center">
  <img src="https://github.com/kamalinux/monty/blob/master/monty.png" alt="Monty logo">
</p>

# 0x19. C - Stacks, Queues - LIFO, FIFO - Monty

Monty is an interpreter of Monty ByteCodes files. Monty 0.98 is a scripting language that is first compiled into Monty byte codes (Just like Python).

## About the Monty language
Monty is a language that aims to close the gap between scripting and programming languages. It contains specific instructions to manipulate data information (stacks or queues), where each instruction (*called opcode*) is sended per line. File contains Monty byte code usually ended by `.m` extension.

## Usage
To compile all files:

```bash
$ gcc -Wall -Werror -Wextra -pedantic *.c -o monty
```

To run the interpreter:

```bash
$ ./monty bytecode_file.m
```

## Features
`monty` executes the following operation codes:

| Opcode | Description |
| -------- | ----------- |
| `push` | Pushes an element to the stack |
| `pall` | Prints all the values on the stack |
| `pint` | Prints the value at the top of the stack |
| `pop` | Removes the top element of the stack |
| `swap` | Swaps the top two elements of the stack |
| `nop` | Doesn't do anything |
| `add` | Adds the top two elements of the stack |
| `sub` | Subtracts the top element of the stack from the second top element of the stack |
| `mul` | Multiplies the second top element of the stack with the top element of the stack |
| `div` | Divides the second top element of the stack by the top element of the stack |
| `mod` | Computes the rest of the division of the second top element of the stack by the top element of the stack |
| `#` | When the first non-space of a line is a # the line will be trated as a comment (don’t do anything) |
| `pchar` | Prints the char at the top of the stack |
| `pstr` | Prints the string starting at the top of the stack |
| `rotl` | Rotates the stack to the top |
| `rotr` | Rotates the stack to the bottom |
| `queue` | Sets the format of the data to a queue (FIFO) |
| `stack` | Sets the format of the data to a stack (LIFO) |

