# Operators

## Learning Goals

- Explain an expression.
- Explain an operator.
- Use common operators (arithmetic, comparison).

## Introduction

In mathematics, we can perform calculations using operators like `+`, `-`, `/`
and so on. Programming languages also provide operators to perform calculations
using values. Here’s an example of addition:

```python
print(4 + 6)
```

Output:

```
10
```

## What is an Expression?

An “expression” in Python is any code that evaluates to a value. A single value
is also an expression. Here are a few examples:

- `1` produces `1`.
- `"Hello!"` produces `"Hello!"`.
- `5 * 2` produces `10`.
- `num > 100` produces either `True` or `False`.

An expression can contain multiple expressions within it. Let’s take a look at a
more complex expression:

```python
(5 + 2) + 3
```

The above line of code has 5 expressions:

- `5` (produces 5)
- `2` (produces 2)
- `3` (produces 3)
- `5 + 2` (produces 7)
- `(5 + 2) + 3` (produces 10)

Here’s the expression used with the `print` function in Python:

```python
print((5 + 2) + 3) # 10
```

The computer evaluates the expression by simplifying it incrementally. Here are
the intermediate steps that are hidden from us:

```python
-> (5 + 2) + 3
-> 7 + 3
-> 10
```

Expressions in parenthesis are evaluated first.

## Arithmetic Operators

These operators are used for performing calculations with numbers (both `int`
and `float`). The following are the arithmetic operators in Python:

| Operator | Description                                                                                         | Syntax   | Results |
| -------- | --------------------------------------------------------------------------------------------------- | -------- | ------- |
| +        | Addition: Adds two operands                                                                         | 5 + 2    | 7       |
| -        | Subtraction: Subtracts two operands                                                                 | 5 - 2    | 3       |
| \*       | Multiplication: Multiplies two operands                                                             | 5 \* 2   | 10      |
| /        | Non-integer division: Divides the first operand by the second and returns a floating point quotient | 5 / 2    | 2.5     |
| //       | Integer division: Divides the first operand by the second, and forces the result to be an integer   | 5 // 2   | 2       |
| %        | Modulo: Returns the remainder when the first operand is divided by the second                       | 5 % 2    | 1       |
| \*\*     | Power: Returns the first number raised to power of the second number.                               | 5 \*\* 2 | 25      |

```python
print(5 + 2)  # 7
print(5 - 2)  # 3
print(5 * 2)  # 10
print(5 / 2)  # 2.5
print(5 // 2) # 2
print(5 % 2)  # 1
print(5 ** 2) # 25
```

## Comparison Operators

These operators are used for comparing values. The values being compared must be
of the same data type. For example, numbers can only be compared with numbers.

| Operator | Description                                                                              | Syntax | Results |
| -------- | ---------------------------------------------------------------------------------------- | ------ | ------- |
| >        | Greater than: True if the left operand is greater than the right                         | 5 > 2  | True    |
| <        | Less than: True if the left operand is less than the right                               | 5 < 2  | False   |
| ==       | Equal to: True if both operands are equal                                                | 5 == 2 | False   |
| !=       | Not equal to: True if both operands are not equal                                        | 5 != 2 | True    |
| >=       | Greater than or equal to: True if the left operand is greater than or equal to the right | 5 >= 2 | True    |
| <=       | Less than or equal to: True if the left operand is less than or equal to the right       | 5 <= 2 | False   |

```python
print(5 > 2)  # True
print(5 < 2)  # False
print(5 == 2) # False
print(5 != 2) # True
print(5 >= 2) # True
print(5 <= 2) # False
```

We will primarily be using comparison operators with numbers in this course. You
can see how strings are compared
[in this article](https://www.digitalocean.com/community/tutorials/python-string-comparison).

## Logical Operators

These operators are used to compare multiple boolean values.

| Operator | Description                                          | Syntax          | Results |
| -------- | ---------------------------------------------------- | --------------- | ------- |
| and      | Logical AND: True only if both the operands are True | 1 > 2 and 2 > 5 | False   |
| or       | Logical OR: True if either of the operands is True   | 1 > 2 or 5 > 2  | True    |
| not      | Logical NOT: flips the boolean value                 | not True        | False   |

Check out this article for
[full truth tables](https://www.digitalocean.com/community/tutorials/understanding-boolean-logic-in-python-3).

## Conclusion

We have learned about expressions and comparison operators in Python. These
operators are fairly common across programming languages.
