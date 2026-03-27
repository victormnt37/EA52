# n-Queens – CSP Modeling (README)

## 1. CSP Modeling (General)

The **n-Queens** problem asks to place _n_ queens on an _n×n_ board so that no two queens attack each other.

### Variables

One variable per row:

- \( x_i \): column of the queen in row \( i \)

### Domains

- \( D(x_i) = \{1, ..., n\} \)

### Constraints

- **Different columns:**  
  \( x_i != x_j \)

- **Different diagonals:**  
  \( |x_i - x_j| != |i - j| \)

This defines the CSP \((X, D, C)\) for any \( n > 3 \).

---

## 2. CSP Instantiation (n = 5)

### Variables

\( X = \{x_1, x_2, x_3, x_4, x_5\} \)

### Domains

Each variable: \( \{1, 2, 3, 4, 5\} \)

### Constraints

For all \( i < j \):

- \( x_i != x_j \)
- \( |x_i - x_j| != |i - j| \)
