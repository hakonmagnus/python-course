# Operators and Precedence

Lecture 13 in the Udemy course discussed operators and their precedence. To remind you, precedence refers to
the order in which operators are evaluated. For example, multiplication is performed before addition. So the following:

```python
a * b + c * d
```

Is the same as this:

```python
(a * b) + (c * d)
```

If you want to change the order, or if you are unsure in which order your expression is evaluated and want to specify
the order yourself, you can use these parentheses as in the example above.

## Precedence Table

The following table lists all the different operators in Python in order. The top of the table is evaluated first,
and the bottom of the table is evaluated last (descending order).

| Operators                   | Description          |
|-----------------------------|----------------------|
| ( )                         | Parentheses          |
| \*\*                        | Exponent             |
| +x, -x, ~x                  | Unary plus, Unary minus, Bitwise NOT |
| \*, /, //, %                | Multiplication, Division, Floor division, Modulus |
| +, -                        | Addition, Subtraction |
| <<, >>                      | Left shift, Right shift |
| &                           | Bitwise AND          |
| ^                           | Bitwise XOR          |
| \|                          | Bitwise OR           |
| ==, !=, >, >=, <, <=, is, is not, in, not in | Comparisons, Identity, Membership |
| not                         | Logical NOT          |
| and                         | Logical AND          |
| or                          | Logical OR           |

Don't worry if you are not familiar with all of these operators, we haven't covered them all. But you can refer
to this table as needed.

## Associativity of Operators

One thing I did not mention about operators is associativity. When two operators have the same precedence, the
associativity helps determine the order of operations. Most operators have left-to-right associativity. There are
only two operators you should know about that have right-to-left associativity, which are the exponent \*\* operator
and the logical not operator. Allow me to demonstrate:

```python
# Left-right associativity
# Calculated as (100 / 10) * 10
# First left, then right
print(100 / 10 * 10)
```