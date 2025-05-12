#### Standard Deviation Calculation Methods

##### Method 1: Using Deviations from Mean

The standard deviation measures how spread out the values are from the mean. Here's the step-by-step method:

##### Step 1: List the values and calculate the mean
Given values: x = 59, 64, 69, 72, 76, 80
Mean = 70 (given). This means that the values and mean are treated as constants throughout the calculation process.

##### Step 2: Calculate the deviation of each value from the mean
- 59 - 70 = -11
- 64 - 70 = -6
- 69 - 70 = -1
- 72 - 70 = 2
- 76 - 70 = 6
- 80 - 70 = 10

##### Step 3: Square each deviation
- (-11)² = 121
- (-6)² = 36
- (-1)² = 1
- (2)² = 4
- (6)² = 36
- (10)² = 100

##### Step 4: Calculate the mean of these squared deviations (variance)
- Sum of squared deviations = 121 + 36 + 1 + 4 + 36 + 100 = 298
- Number of values = 6
- Variance = 298 ÷ 6 = 49.67

##### Step 5: Take the square root of the variance
- Standard deviation = √49.67 ≈ 7.05

#### Method 2: Using Mean of Squares

##### Step 1: Square each value
- 59² = 3,481
- 64² = 4,096
- 69² = 4,761
- 72² = 5,184
- 76² = 5,776
- 80² = 6,400

##### Step 2: Find the sum of the squared values
- 3,481 + 4,096 + 4,761 + 5,184 + 5,776 + 6,400 = 29,698

##### Step 3: Calculate the mean of the squared values
- 29,698 ÷ 6 = 4,949.67

##### Step 4: Calculate the square of the mean
- 70² = 4,900

##### Step 5: Subtract the square of the mean from the mean of squares
- 4,949.67 - 4,900 = 49.67

##### Step 6: Take the square root of this result
- √49.67 ≈ 7.05

This method uses the standard deviation formula

$$
\sigma = \sqrt{\frac{\sum x^2}{n} - \left(\frac{\sum x}{n}\right)^2}
$$

which is another way to calculate variance. Here, Σ(x²)/n is the "mean of squares," and (Σx/n)² is the "square of the mean."

#### Why These Methods Are Equivalent?

First method (mean of squared deviations):

$$
\\sigma^2 = \\frac{\\sum(x - \\mu)^2}{n}
$$

Second method (mean of squares minus square of the mean):

$$
\\sigma^2 = \\frac{\\sum x^2}{n} - \\left(\\frac{\\sum x}{n}\\right)^2
$$

Let's prove these are equivalent by expanding the first formula:

$$
\\frac{\\sum(x - \\mu)^2}{n}
$$

Expanded:

$$
= \\frac{\\sum(x^2 - 2x\\mu + \\mu^2)}{n}
$$

$$
= \\frac{\\sum x^2}{n} - \\frac{2\\mu\\sum x}{n} + \\frac{\\sum \\mu^2}{n}
$$

Since $\\mu = \\frac{\\sum x}{n}$ and $\\mu$ is a constant:

$$
= \\frac{\\sum x^2}{n} - 2\\mu \\left(\\frac{\\sum x}{n}\\right) + \\mu^2
$$

$$
= \\frac{\\sum x^2}{n} - 2 \\left(\\frac{\\sum x}{n}\\right)^2 + \\left(\\frac{\\sum x}{n}\\right)^2
$$

$$
= \\frac{\\sum x^2}{n} - \\left(\\frac{\\sum x}{n}\\right)^2
$$



#### Simplified Proof (Substituting μ with a Constant A)

We can substitute the mean $\mu = \frac{\sum x}{n}$ with a constant $A$ (e.g., $A = 70$ in a given dataset).

1. Start from Method 1:

$$
\sigma^2 = \frac{\sum (x - A)^2}{n}
$$

2. Expand the squared term:

$$
\sigma^2 = \frac{\sum (x^2 - 2xA + A^2)}{n}
$$

3. Apply the distributive property of summation:

$$
\sigma^2 = \frac{\sum x^2 - \sum 2xA + \sum A^2}{n}
$$

4. Factor out the constant $A$ from the summation:

$$
\sigma^2 = \frac{\sum x^2 - 2A\sum x + nA^2}{n}
$$

5. Divide each term by $n$:

$$
\sigma^2 = \frac{\sum x^2}{n} - 2A \cdot \frac{\sum x}{n} + A^2
$$

6. Substitute $A = \frac{\sum x}{n}$:

$$
\sigma^2 = \frac{\sum x^2}{n} - 2A \cdot A + A^2
$$

7. Simplify:

$$
\sigma^2 = \frac{\sum x^2}{n} - 2A^2 + A^2 = \frac{\sum x^2}{n} - A^2
$$

8. Re-substitute $A = \frac{\sum x}{n}$:

$$
\sigma^2 = \frac{\sum x^2}{n} - \left( \frac{\sum x}{n} \right)^2
$$

This final expression matches exactly with Method 2. Therefore, both methods for calculating variance are mathematically equivalent.


