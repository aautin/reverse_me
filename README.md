# Reverse Me - Binary Analysis Challenge

A multi-level reverse engineering challenge featuring progressively complex binary analysis tasks. Each level contains a binary that must be analyzed to discover hidden passwords.

## Challenge Overview

This project contains 3 levels of reverse engineering challenges, each with increasing complexity:

```mermaid
flowchart TD
    A[Level 1: Basic String Comparison] --> B[Level 2: Conditional Logic Analysis]
    B --> C[Level 3: Advanced Binary Analysis]
    
    A1[Binary Analysis] --> A2[String Extraction]
    A2 --> A3[Password: __stack_check]
    
    B1[Control Flow Analysis] --> B2[Conditional Branches]
    B2 --> B3[Multi-step Validation]
    
    C1[Complex Assembly] --> C2[Advanced Techniques]
    C2 --> C3[Sophisticated Password]
```

## Project Structure

```
reverse_me/
├── binary/          # Compiled binaries for each level
│   ├── level1       # Basic string comparison challenge
│   ├── level2       # Conditional logic challenge
│   └── level3       # Advanced binary analysis
├── levelX/          # Level X analysis materials
│   ├── source.c     # Reimplementation from scratch
│   ├── workflow.md  # Detailed analysis workflow
│   └── password     # Solution
...
```

## Analysis Methodology

Each level demonstrates different reverse engineering techniques:

- **Level 1**: Basic string comparison using `strcmp()` - Introduces fundamental binary analysis
- **Level 2**: Conditional logic with multiple validation steps - Explores control flow analysis
- **Level 3**: Advanced binary analysis requiring sophisticated reverse engineering techniques

## Tools & Requirements

- **GDB**: GNU Debugger for dynamic analysis
- **objdump**: Object file analyzer for disassembly  
- **strings**: Extract printable strings from binaries
- **hexdump**: Hex viewer for binary inspection
- **IDA Pro/Ghidra**: Advanced reverse engineering platforms (optional)
- Linux environment with debugging capabilities