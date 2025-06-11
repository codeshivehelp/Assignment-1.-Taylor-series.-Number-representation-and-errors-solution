# Assignment-1.-Taylor-series.-Number-representation-and-errors-solution

Download Here: [Assignment 1. Taylor series. Number representation and errors solution](https://jarviscodinghub.com/assignment/assignment-1-taylor-series-number-representation-and-errors-solution/)

For Custom/Original Work email jarviscodinghub@gmail.com/whatsapp +1(541)423-7793

Problem 1. (computer) (2 points)
Study the following central difference formula:
f 0
(x) ⇡ f(x+h) f(xh)
2h
as h ! 0. Using Taylor’s theorem, we obtain that the truncation error for this formula is
h2
6 f 000(x) for some x in the interval (xh, x+h). In a computer, the result is also subject
to a rounding error. The total error is given by the sum of these two errors.
Write and run a code which computes the approximate values of the truncation error and
the total error as a function of h for f(x) = sin(x) at x = 0.5. On the same graph, plot
the results showing the rounding error (er), the truncation error (et) and the total error
(e = er + et). Use log-scale, i.e. plot log10 h (x-axis) vs. log10 |error| (y-axis). Analyze
the results. (Hint: start with an initial value of h, e.g. h = 0.5, and divide the value of h at
each step by some factor, e.g. h h/4).
Problem 2. (pencil and paper) (0 points – do not return)
Suppose that you have a floating-point system in which numbers are represented in the
following form
x = ±0.d1d2d3d4 ⇥10n
where the exponent n is a 2-digit (decimal) integer and the normalized mantissa has four
digits d1d4. Use this system to compute the difference pq where p = 75640 and q = 4.
1
Problem 3. (pencil and paper / computer) (2 points)
(a) The harmonic series 1 + 1
2 + 1
3 + 1
4 + … is known to diverge to +•. The nth partial
sum approaches +• at the same rate as ln(n). Euler’s constant is defined to be
g = lim
n!•
” n
Â
k=1
1
k ln(n)
#
⇡ 0.57721
Write and test a program that uses a loop of 5000 steps to estimate Euler’s constant. Print
intermediate answers at every 100 steps. Compare to exact value.
(b) Prove (using pencil and paper) that Euler’s constant can also be presented by
g = lim
m!•
” m
Â
k=1
1
k ln(m+
1
2
)
#
Write and test a program that uses m = 1,2,3,…,5000 to compute g by this formula.
Compare the convergence to the formula given in part (a). For those interested, see
D.W.Temple, “A quicker convergence to Euler’s constant”, Am. Math. Monthly 100,
468 (1993).
Problem 4. (pencil and paper) (0 points – do not return)
Let us have a floating-point representation in which the numbers x are expressed in the
following form
x = ±(0.b1b2b3)2 ⇥2±m m,bi = {0,1}
List all positive numbers that are representable using this form. (You can form a table of
the mantissa and the exponent bits and convert the combination into base 10 numbers).
What if the representation is normed (the first bit b1 is always 1)?
Problem 5. (2 points) (computer)
Using a computer, examine how the computed values of the following functions behave
near the point x = 0.
(a) f1(x) = ex 1
x
(b) f2(x) = ex ex
2x
In order to avoid loss of significance as a result of subtracting almost equal numbers, expand the exponential functions into Taylor series and use the resulting approximation to
calculate the values of the functions f1 and f2 near zero. Estimate the error of the approximation by using Taylor’s theorem on the series expansion of the exponential function
(f(x) = ex):
f(x) = f(0) +
n1
Â
i=1
xi
i!
f (i)
(0) +R(n)
where the error term is
R(n) = xn
n!
f (n)
(x) 0  x  x
2
