---
title: Calculus Progress
date: 2025-03-20 00:00:00 +0800
categories: [Math,Studies]
tags: [Calculus, Limit, Riemann Sum]
---

# What I Learn
In today's class, I'm learning more about limits and the concept of **Riemann sums** as an approach to integration.

# Riemann Sum
The **Riemann Sum** is a method for approximating the total area underneath a curve on a graph—an essential idea in integral calculus. It works by dividing the area under a function into small rectangles, calculating the area of each, and summing them together.

For a function \( f(x) \) on the interval \([a, b]\), we divide the interval into \( n \) subintervals of equal width:

\[
\Delta x = \frac{b - a}{n}
\]

Then, we choose sample points \( x_i^* \) in each subinterval \([x_{i-1}, x_i]\), and compute the sum of areas of the rectangles formed by these points:

\[
\sum_{i=1}^{n} f(x_i^*) \cdot \Delta x
\]

There are several common types of Riemann sums based on the choice of \( x_i^* \):
- **Left Riemann Sum**: Uses the left endpoint of each subinterval.
- **Right Riemann Sum**: Uses the right endpoint.
- **Midpoint Riemann Sum**: Uses the midpoint of each subinterval.

As the number of subintervals increases (i.e., \( n \to \infty \)), the Riemann sum becomes a better approximation of the **definite integral**:

\[
\int_a^b f(x)\,dx = \lim_{n \to \infty} \sum_{i=1}^{n} f(x_i^*) \cdot \Delta x
\]

This limit, when it exists, gives the exact area under the curve \( f(x) \) between \( a \) and \( b \).

---

