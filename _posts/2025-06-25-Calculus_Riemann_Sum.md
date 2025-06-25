---
title: Calculus Progress 2
date: 2025-06-25 00:00:00 +0800
categories: [Math,Studies]
tags: [Calculus, Limit, Riemann Sum]
---

# What I Learn
In today's class, I'm learning more about limits and the concept of Riemann sums as an approach to integration.

# Riemann Sum
The **Riemann Sum** is a method for approximating the total area underneath a curve on a graph, otherwise known as an integral. It's based on summing up areas of multiple rectangles beneath the curve.

For a function \( f(x) \) on the interval \([a, b]\), we divide the interval into \( n \) subintervals of equal width \( \Delta x = \frac{b - a}{n} \), and then choose sample points \( x_i^* \) in each subinterval. The Riemann Sum is given by:

\[
\sum_{i=1}^{n} f(x_i^*) \Delta x
\]

There are several types of Riemann Sums, depending on how the sample point \( x_i^* \) is chosen:
- **Left Riemann Sum**: \( x_i^* \) is the left endpoint.
- **Right Riemann Sum**: \( x_i^* \) is the right endpoint.
- **Midpoint Riemann Sum**: \( x_i^* \) is the midpoint.

As \( n \to \infty \), the Riemann Sum approaches the **definite integral**:

\[
\int_a^b f(x) \, dx = \lim_{n \to \infty} \sum_{i=1}^{n} f(x_i^*) \Delta x
\]

This forms the basis of integral calculus, allowing us to compute exact areas under curves when the function is integrable.
