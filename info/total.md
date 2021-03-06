We have found an interesting algorithm for optimisation of the fuel system.
If we will divide the fuel rod for the several parts by the Triangular numbers law,
then we will get more power.

Our goal is to divide the fuel rod in several pieces. The length of the rod is **N** metres.
All of the parts should have integer lengths (1, 2, 3 .. metres, but not 1.2).

You should divide the stick so that the lengths form 
the consecutive fragment of [the Triangular numbers](http://en.wikipedia.org/wiki/Triangular_number) 
series with the maximum quantity (fragment's length).
The parts should have different lengths (no repeating).
For example: **64** should divided at **15, 21, 28**,
because **28, 36** is shorter and **1, 3, 15, 45** is not a consecutive fragment.

You are given a length of the stick (N).
You should return the list of lengths (integers) for the parts in ascending order.
If it's not possible and the problem does not have a solution, then you should return an empty list.

![Rods](sawing.png)

**Input:** A length of the rod as an integer. 

**Output:** A fragment of the Triangular numbers as a list of integers (sorted in ascending order) or an empty list.

**Example:**

```python
disjoint(64) == [15, 21, 28]
disjoint(371) == [36, 45, 55, 66, 78, 91]
disjoint(225) == [105, 120]
disjoint(882) == []
```
**How it is used:**

In this task you will learn about triangular numbers.
A triangular number or triangle number counts the objects that form an equilateral triangle.
This is an interesting sequence which has various applications.

Here’s a real world application:
In a competitive tournament format that uses a round-robin group stages,
the number of matches that need to be played between n teams is equal to the triangular number T<sub>n−1</sub>.
For example, a group stage with 4 teams requires 6 matches, and a group stage with 8 teams requires 28 matches.

**Precondition:**
```python
0 < length < 1000
```
