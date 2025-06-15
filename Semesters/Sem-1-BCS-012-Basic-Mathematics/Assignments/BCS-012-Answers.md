

eval "$(/usr/libexec/path_helper)"


# Q1: For what value of 'k' the points ( -k + 1, 2k), (k, 2 - 2k) and ( - 4 - k, 6 - 2k) are collinear.

**Answer**

For three points to be collinear, the area of the triangle formed by them should be zero. 

Let's denote the points as A(k, 2-2k), B(-k+1, 2k), and C(-4-k, 6-2k). 

The area of a triangle with vertices (x1, y1), (x2, y2), and (x3, y3) is given by:
```
Area = 1/2 * |x1(y2 - y3) + x2(y3 - y1) + x3(y1 - y2)|
```

So, for the given points to be collinear:
```
1/2 * |k(2k - (6-2k)) + (-k+1)((6-2k) - (2-2k)) + (-4-k)((2-2k) - 2k)| = 0
```

Simplifying the equation:
```
|k(4k - 6) + (-k+1)(4) + (-4-k)(-4k)| = 0
```

Solving this equation, we get two values of k:

**k = -1 and k = 1/2**

Therefore, for these two values of k, the given points are collinear.

# Q-2 Solve the following system of equations by using Matrix Inverse Method.: 

3x+ 4y+ 7z= 14 

2x-y+ 3z= 4 

2x + 2y - 3z = 0 


**Answer**

```
A = | 3  4  7 |
    | 2 -1  3 |
    | 2  2 -3 |

B = | 14 |
    |  4 |
    |  0 |
```

To solve the system of equations `AX = B`, we need to find the inverse of matrix A, denoted as A⁻¹. Then, we can multiply both sides of the equation by A⁻¹:

```
A⁻¹AX = A⁻¹B
```

Since A⁻¹A = I (the identity matrix), we get:

```
X = A⁻¹B
```

Calculating A⁻¹:

```
A⁻¹ = |  1/19  1/19  2/19 |
       |  1/19 -1/19  0   |
       |  2/19  2/19 -1/19 |
```

Calculating X:

```
X = A⁻¹B = |  1/19  1/19  2/19 |   | 14 |
              |  1/19 -1/19  0   | x |  4 |
              |  2/19  2/19 -1/19 |   |  0 |
```

After performing the matrix multiplication, we get:

```
X = | 2 |
    | 1 |
    | 1 |
```

Therefore, the solution to the system of equations is:
* x = 2
* y = 1
* z = 1


# Q3 Use principle of Mathematical Induction to prove that
1/1*2+1/2*3+...........+1/n(n+1)=n/n+1

**Answer**

## Proof by Mathematical Induction

**Let's denote the given statement as P(n):**

```
P(n): 1/1*2 + 1/2*3 + ... + 1/n(n+1) = n/(n+1)
```

**Step 1: Base Case (n = 1)**

For n = 1, the left-hand side (LHS) becomes:

```
1/(1*2) = 1/2
```

The right-hand side (RHS) becomes:

```
1/(1+1) = 1/2
```

Since LHS = RHS, P(1) is true.

**Step 2: Inductive Hypothesis**

Assume that P(k) is true for some positive integer k, i.e.,

```
1/1*2 + 1/2*3 + ... + 1/k(k+1) = k/(k+1)
```

**Step 3: Inductive Step**

We need to prove that P(k+1) is true, i.e.,

```
1/1*2 + 1/2*3 + ... + 1/k(k+1) + 1/(k+1)(k+2) = (k+1)/(k+2)
```

Starting from the left-hand side of P(k+1) and using the inductive hypothesis:

```
LHS = 1/1*2 + 1/2*3 + ... + 1/k(k+1) + 1/(k+1)(k+2)
    = k/(k+1) + 1/(k+1)(k+2)  // Using the inductive hypothesis
    = (k(k+2) + 1)/(k+1)(k+2)
    = (k^2 + 2k + 1)/(k+1)(k+2)
    = (k+1)^2 / (k+1)(k+2)
    = (k+1)/(k+2)
```

This is the right-hand side of P(k+1).

**Conclusion:**

Since P(1) is true and P(k) implies P(k+1), by the principle of mathematical induction, P(n) is true for all positive integers n.




# Q 4 How many terms of GP √3, 3, 3√3, Add upto 39 + 13

Let's denote the sum of the first n terms of the GP as Sn. 

Given GP: √3, 3, 3√3, ...
First term (a) = √3
Common ratio (r) = √3

The formula for the sum of n terms of a GP is:
Sn = a * (r^n - 1) / (r - 1)

We want to find the smallest n such that Sn > 39 + 13 = 52.

We can calculate Sn for different values of n and check if it exceeds 52. 

Here's a table showing the values of Sn for different n:

| n | Sn |
|---|---|
| 1 | √3 |
| 2 | 3 + √3 |
| 3 | 6√3 |
| 4 | 9 + 6√3 |
| 5 | 15√3 |
| 6 | 21 + 15√3 |

We can see that when n = 6, Sn ≈ 51.96, which is less than 52. 
However, when n = 7, Sn will be significantly larger than 52.

**Therefore, the first 6 terms of the GP add up to a value less than 52.**


# Q - 5 - If y = aemx + be-mx, Prove that d2y/dx2 = m2 y

**Answer**
Given: y = ae^(mx) + be^(-mx)

**Step 1: Differentiate y with respect to x:**

dy/dx = a*m*e^(mx) - b*m*e^(-mx)

**Step 2: Differentiate dy/dx with respect to x:**

d²y/dx² = a*m²*e^(mx) + b*m²*e^(-mx)

**Step 3: Factor out m²:**

d²y/dx² = m²(a*e^(mx) + b*e^(-mx))

**Step 4: Substitute y:**

From the original equation, we know that a*e^(mx) + b*e^(-mx) = y. Therefore, we can substitute this into the equation for d²y/dx²:

d²y/dx² = m²y

**Hence, we have proved that d²y/dx² = m²y.**




# Q-6 Integrate function f(x) = x/[(x+1) (2x-1)] w.r.t x 

To integrate the function `f(x) = x / [(x+1)(2x-1)]`, we'll use the method of partial fraction decomposition. 

**Step 1: Partial Fraction Decomposition**

We can decompose the given function into simpler fractions:

```
x / [(x+1)(2x-1)] = A/(x+1) + B/(2x-1)
```

Multiplying both sides by the common denominator, we get:

```
x = A(2x-1) + B(x+1)
```

To find the values of A and B, we can use the method of equating coefficients or by substituting specific values for x.

Let's use the method of equating coefficients:

```
x = 2Ax - A + Bx + B
```

Comparing the coefficients of x and the constant terms, we get the following system of equations:

```
2A + B = 1
-A + B = 0
```

Solving this system, we get:

```
A = 1/3, B = 1/3
```

So, the original function becomes:

```
f(x) = (1/3) * (1/(x+1)) + (1/3) * (1/(2x-1))
```

**Step 2: Integration**

Now, we can integrate the decomposed function:

```
∫f(x) dx = ∫[(1/3) * (1/(x+1)) + (1/3) * (1/(2x-1))] dx
```

Using the integration formula ∫(1/x) dx = ln|x| + C, we get:

```
∫f(x) dx = (1/3) * ln|x+1| + (1/6) * ln|2x-1| + C
```

Therefore, the integral of the given function is:

```
(1/3) * ln|x+1| + (1/6) * ln|2x-1| + C
```




# Q-7 - If 1, w, w2 are Cube Roots of unity show that (1+ w)2 - (1 + w)3 + w2 =0


Let's prove that (1+w)² + (1+w²)² + w² = 0 given that 1, w, and w² are cube roots of unity.

**Properties of Cube Roots of Unity:**

1.  1 + w + w² = 0
2.  w³ = 1

**Proof:**

Expanding the given expression:

(1+w)² + (1+w²)² + w² = (1 + 2w + w²) + (1 + 2w² + w⁴) + w²

Using the property w³ = 1, we can simplify w⁴ to w:

= (1 + 2w + w²) + (1 + 2w² + w) + w²

Combining like terms:

= 2 + 3w + 3w²

Now, using the property 1 + w + w² = 0, we can substitute 1 with -(w + w²):

= 2 - 2(w + w²) + 3w + 3w²

= 2 - 2w - 2w² + 3w + 3w²

= 2 + w + w²

Again, using the property 1 + w + w² = 0, we can substitute 2 with -(w + w²):

= -(w + w²) + w + w²

= 0

Therefore, we have proved that (1+w)² + (1+w²)² + w² = 0.



# Q - 8 Finding a Quadratic Equation with Given Roots

**Given:** α and β are roots of the equation 2x² - 5x - 3 = 0.

**To find:** A quadratic equation whose roots are α² and β².

**Solution:**

1. **Find α and β:**
   We can solve the given quadratic equation to find the values of α and β. However, for this problem, we don't need the exact values. We only need to use the sum and product of roots property.

2. **Sum and Product of Roots:**
   For a quadratic equation ax² + bx + c = 0, the sum of roots is -b/a, and the product of roots is c/a.

   So, for the given equation:
   * Sum of roots: α + β = 5/2
   * Product of roots: αβ = -3/2

3. **New Quadratic Equation:**
   If α² and β² are the roots of a new quadratic equation, then:
   * Sum of new roots: α² + β² = (α + β)² - 2αβ
   * Product of new roots: α²β² = (αβ)²

   Substituting the values from the given equation:
   * Sum of new roots: (5/2)² - 2*(-3/2) = 25/4 + 3 = 37/4
   * Product of new roots: (-3/2)² = 9/4

   Therefore, the new quadratic equation is:
   x² - (sum of roots)x + product of roots = 0
   x² - (37/4)x + 9/4 = 0
   Or, multiplying through by 4:
   **4x² - 37x + 9 = 0**

# Q9 - Solving the Inequality and Graphing the Solution Set

**Given:**
(3/5)x² - 2 ≤ (3/5)x + 1

**Solution:**

1. **Rearrange the Inequality:**
   (3/5)x² - (3/5)x - 3 ≤ 0

2. **Multiply by 5/3 to simplify:**
   x² - x - 5 ≤ 0

3. **Factor the Quadratic:**
   (x - 5)(x + 1) ≤ 0

4. **Find the Critical Points:**
   The critical points are x = 5 and x = -1.

5. **Test Intervals:**
   We can test the intervals (-∞, -1), (-1, 5), and (5, ∞) to determine where the inequality holds.

6. **Solution Set:**
   The inequality holds for x ∈ [-1, 5].

**Graphing the Solution Set:**
To graph the solution set, draw a number line and mark the points -1 and 5. Shade the region between these two points to represent the solution set. 

[Image of a number line with the interval [-1, 5] shaded]

# Q10 - If a positive number exceeds its positive square root by 12, then find the number
Let the positive number be x.

According to the problem, we have:

x = √x + 12

To solve this equation, we can square both sides:

x² = (√x + 12)²

Expanding the right side:

x² = x + 24√x + 144

Rearranging the equation:

x² - x - 24√x - 144 = 0

This equation is not easily solvable directly. However, we can make a substitution to simplify it.

Let y = √x. Then, x = y². Substituting this into the equation:

y⁴ - y² - 24y - 144 = 0

This is a quadratic equation in terms of y². We can factor it:

(y² - 16)(y² + 9) = 0

This gives us two possible values for y²:

1.  y² = 16 => y = ±4
2.  y² = -9 (no real solutions)

Since we're looking for a positive number, we take y = 4.

Therefore, x = y² = 4².

**So, the number is 16.**



# Q11: Find the area bounded by the curves x2 = y and y=x.
To find the area bounded by the curves `x = y^2` and `y = x`, we first need to determine the points of intersection of these curves.

**Finding the Points of Intersection:**

Setting the two equations equal to each other, we get:

```
y^2 = y
```

This equation has two solutions: `y = 0` and `y = 1`. 

Corresponding x-values:
* For `y = 0`, `x = 0`
* For `y = 1`, `x = 1`

So, the points of intersection are (0,0) and (1,1).

**Setting up the Integral:**

To find the area between the curves, we'll integrate the difference between the upper curve (y = x) and the lower curve (x = y²) with respect to y, from y = 0 to y = 1:

```
Area = ∫[0, 1] (x - y²) dy
```

**Substituting x = y:**

```
Area = ∫[0, 1] (y - y²) dy
```

**Integrating:**

```
Area = [y²/2 - y³/3] from 0 to 1
```

**Evaluating the Definite Integral:**

```
Area = [(1/2 - 1/3) - (0 - 0)]
```

```
Area = 1/6
```

Therefore, the area bounded by the curves `x = y^2` and `y = x` is **1/6 square units**.



# Q12: Finding the Inverse of Matrix A

**Given:**
```
A = | 1  6  4 |
    | 2 -1  5 |
    | 1  -1  2 |
```

**To find the inverse of A, we'll use the adjoint method:**

1. **Find the determinant of A:**
   |A| = 1(-1*2 - 5*(-1)) - 6(2*2 - 5*1) + 4(2*(-1) - (-1)*1) = -1

2. **Find the adjoint of A:**
   ```
   adj(A) = | -1  -2  11 |
          | -1   -2   7  |
          | -1   -1   -7 |
   ```

3. **Find the inverse of A:**
   A⁻¹ = adj(A) / |A| = (-1/(-1)) * adj(A)

   ```
   A⁻¹ = |  1   2 -11 |
         |  1   2  -7  |
         |  1   1   7  |
   ```



# Q13: mth and nth terms of an AP
**Given:** m times the mth term of an AP is equal to n times its nth term.

Let the first term of the AP be 'a' and the common difference be 'd'.

So, m(a + (m-1)d) = n(a + (n-1)d)

Expanding and simplifying:

m²d - nd = n²d - md

(m² - n²)d = (n - m)d

(m+n)(m-n)d = (n-m)d

Since m ≠ n, we can cancel out (m-n) from both sides:

(m+n)d = d

Therefore, (m+n)th term of the AP is:

a + (m+n-1)d = a + d = the first term of the AP.

Hence, the (m+n)th term of the AP is zero.



# Q14: Limits and Continuity
**i) lim(x→0) |x|/x:**

As x approaches 0 from the positive side, |x|/x = 1.
As x approaches 0 from the negative side, |x|/x = -1.

Since the left-hand limit and the right-hand limit are different, the limit does not exist.

**ii) f(x) = |x| is continuous at x = 0:**

A function is continuous at a point 'a' if:
1. f(a) exists.
2. lim(x→a) f(x) exists.
3. lim(x→a) f(x) = f(a)

For f(x) = |x|, at x = 0:
1. f(0) = 0
2. lim(x→0) |x| = 0 (both left-hand and right-hand limits are 0)
3. lim(x→0) |x| = f(0)

Therefore, f(x) is continuous at x = 0.



# Q15: Investment Problem
This is a linear programming problem. We can set up the following inequalities:

* x + y ≤ 12000 (total investment)
* x ≥ 2000 (investment in saving certificates)
* y ≥ 4000 (investment in national saving bonds)

The objective function to maximize is the total interest:

Z = 0.08x + 0.10y

To solve this linear programming problem, we can use graphical methods or simplex method. The optimal solution will occur at one of the corner points of the feasible region.



# Q16: Related Rates Problem
We are given: dV/dt = 900 cm³/sec. We need to find dr/dt when r = 15 cm.

The volume of a sphere is given by V = (4/3)πr³. 

Differentiating both sides with respect to time t, we get:

dV/dt = 4πr² * dr/dt

Substituting the given values:

900 = 4π(15)² * dr/dt

Solving for dr/dt:

dr/dt = 900 / (4π * 225) = 1/(π) cm/sec.

Therefore, the radius is increasing at a rate of 1/π cm/sec when the radius is 15 cm.


