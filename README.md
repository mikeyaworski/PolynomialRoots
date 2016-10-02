# Polynomial Roots

## Overview

A Java class that is used to calculate the rational roots of a polynomial. Note that this only works for polynomials that have at least one integer factor.

## Methods

- `static List<Double> getRoots(List<Double> coefficients)` returns the List of roots from the polynomial interpreted from the List of coefficients. The List of coefficients parameter assumes the leading coefficient of the polynomial is at index 0, and the last index of the List is the constant term of the polynomial.  

## Usage

Just download this class and paste it directly into your project.

## Examples

```java
List<Double> coefficients;

// quartic
coefficients = new ArrayList<Double>();
coefficients.add(1d);
coefficients.add(8d);
coefficients.add(4d);
coefficients.add(-48d);
coefficients.add(0d);
System.out.println(Roots.getRoots(coefficients)); // [-6.0, -4.0, 0.0, 2.0]

// cubic
coefficients = new ArrayList<Double>();
coefficients.add(2d);
coefficients.add(3d);
coefficients.add(-17d);
coefficients.add(-30d);
System.out.println(Roots.getRoots(coefficients)); // [-2.5, -2.0, 3.0]

// quadratic
coefficients = new ArrayList<Double>();
coefficients.add(2d);
coefficients.add(9d);
coefficients.add(10d);
System.out.println(Roots.getRoots(coefficients)); // [-2.5, -2.0]

// linear
coefficients = new ArrayList<Double>();
coefficients.add(9d);
coefficients.add(10d);
System.out.println(Roots.getRoots(coefficients)); // [-1.1111111111111112]

// constant
coefficients = new ArrayList<Double>();
coefficients.add(5d);
System.out.println(Roots.getRoots(coefficients)); // []
```
