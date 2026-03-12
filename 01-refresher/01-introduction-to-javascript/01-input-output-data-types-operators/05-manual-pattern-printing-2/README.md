# Manual Pattern Printing - 2

## Problem

Print the following pattern:

```
    *
   **
  ***
 ****
*****
```

## Output Format

Each line contains decreasing spaces and increasing stars.

```
    *
   **
  ***
 ****
*****
```

## Example Output

```
    *
   **
  ***
 ****
*****
```

## Approach

The pattern consists of:

Spaces decreasing from **4 → 0**
Stars increasing from **1 → 5**

Use nested loops:

* Outer loop for rows
* One loop for spaces
* One loop for stars

## Time Complexity

O(n²)

## Space Complexity

O(1)

## Code

See `solution.js`

## Tags

Patterns, Loops
