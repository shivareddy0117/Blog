---
layout: shiva
title:  "Calculus for DataScientist: Understandin Limits"
date:   2024-04-28 12:43:25 -0500
categories: education calculus data-science
parmalink: "Math-for-DataScientists"
---
## Overview

The concept of limit of a function is one of the fundamental ideas that distinguishes calculus from algebra and trigonometry.

## Definition

### Informal Definition of Limit

Let \( f(x) \) be defined on an open interval about \( $ x_0 $ \), _except possibly at_ \( $ x_0 $ \) itself. If \( f(x) \) gets arbitrarily close to \( L \) for all \( x \) sufficiently close to \( $ x_0 $ \), we say that \( f \) approaches the **limit** \( L \) as \( x \) approaches \( $ x_0 $ \), and we write

$$
\lim_{x \to x_0} f(x) = L.
$$

## Theorem 1

### Properties of Limits

The following rules hold if ( $$ \lim_{x \to c} f(x) = L $$ ) and ( $$ \lim_{x \to c} g(x) = M $$ ) ( L and M real numbers).

1. **Sum Rule**:
   $$
   \lim_{x \to c} [f(x) + g(x)] = L + M
   $$

2. **Difference Rule**:
   $$
   \lim_{x \to c} [f(x) - g(x)] = L - M
   $$

3. **Product Rule**:
   $$
   \lim_{x \to c} [f(x) \cdot g(x)] = L \cdot M
   $$

4. **Constant Multiple Rule**:
   $$
   \lim_{x \to c} k f(x) = kL \quad \text{(any number } k)
   $$

5. **Quotient Rule**:
   $$
   \lim_{x \to c} \frac{f(x)}{g(x)} = \frac{L}{M}, \quad M \neq 0
   $$

6. **Power Rule**:
   If \( m \) and \( n \) are integers, then
   $$
   \lim_{x \to c} [f(x)]^{m/n} = L^{m/n},
   $$
   provided ($$ L^{m/n} $$) is a real number.
