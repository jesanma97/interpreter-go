# Pratt Parsing with Top-Down Operator Precedence

This repository contains an implementation of a Pratt parser using the **Top-Down Operator Precedence** method. This approach is particularly useful for parsing mathematical expressions and other programming language constructs with operators that have different levels of precedence and associativity. Additionally, the repository includes an interpreter that evaluates a string by analyzing and categorizing each of its components to understand their functionality.

## Table of Contents

- [Overview](#overview)
  - [Pratt Parsing](#pratt-parsing)
  - [Top-Down Operator Precedence](#top-down-operator-precedence)
  - [String Interpreter](#string-interpreter)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
  - [Running](#running)
  - [Testing](#testing)

## Overview

### Pratt Parsing

The Pratt method is a powerful and flexible parsing technique that simplifies handling operator precedence and associativity in a recursive descent parser. By associating specific parsing functions with different operators and token types, the parser can construct an Abstract Syntax Tree (AST) that reflects the hierarchical structure of the expressions.

### Top-Down Operator Precedence

The **Top-Down Operator Precedence** technique, popularized by Vaughn Pratt, allows the parser to determine operator precedence while parsing expressions from the top down, building the AST as it progresses. This approach is efficient and easy to implement for complex expressions with multiple operators of varying precedences.

### String Interpreter

The accompanying interpreter in this repository takes a string of text and breaks it down into its basic components, categorizing each word or symbol based on its type (e.g., operators, literals, identifiers, etc.). The interpreter then analyzes the structure and functionality of these components within the context of the language, evaluating the final result.

## Features

- **Pratt Parser**: Complete implementation of the Pratt method for parsing complex expressions.
- **Top-Down Operator Precedence**: Manages operator precedence to ensure correct syntactic analysis.
- **Lexical Categories**: Classification of words and symbols in the input string according to their role in the language.
- **Evaluation**: Analysis and evaluation of the behavior of each component within the expression.

## Installation

To get started, clone this repository to your local machine:

```bash
git clone https://github.com/jesanma97/interpreter-go.git
cd interpreter-go
```

## Usage

### Running

You can run the interpreter by providing the next command:

```bash
go run main.go
```
The text is shown below:
Feel free to type in commands

Now you can enter the expression that will tell you the type of each element, for example:
```
(3 + 4) - 6
```
The result is:
```
{Type:( Literal:(}
{Type:INT Literal:3}
{Type:+ Literal:+}
{Type:INT Literal:4}
{Type:) Literal:)}
{Type:- Literal:-}
{Type:INT Literal:6}
```


### TESTING

To run tests for the parser and interpreter, use the following command:

```bash
go go test ./...
```

