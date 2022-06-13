# Fast Relaxed Vector Fitting for Truncated Signals 

The `vectfit` function approximates a response ![fs](https://latex.codecogs.com/gif.latex?\mathbf{f}(s))
(generally a vector) with a rational function:

![vf](https://latex.codecogs.com/gif.latex?\mathbf{f}(s)&space;\approx&space;\sum_{j=1}^{N}&space;\frac{\mathbf{r}_j}{s-p_j}&space;&plus;&space;\sum_{n=0}^{Nc}&space;\mathbf{c}_n&space;s^{n})

where ![pj](https://latex.codecogs.com/gif.latex?p_j) and
![rj](https://latex.codecogs.com/gif.latex?r_j) are poles and residues in
the complex plane and ![cn](https://latex.codecogs.com/gif.latex?c_n) are
the polynomial coefficients.
When ![fs](https://latex.codecogs.com/gif.latex?\mathbf{f}(s)) is a vector, all
elements become fitted with a common pole set.

The identification is done using the pole relocating method known as Vector
Fitting [1] with relaxed non-triviality constraint for faster convergence
and smaller fitting errors [2], and utilization of matrix structure for fast
solution of the pole identifion step.

- [1] B. Gustavsen and A. Semlyen, "Rational approximation of frequency
    domain responses by Vector Fitting", IEEE Trans. Power Delivery,
    vol. 14, no. 3, pp. 1052-1061, July 1999.
- [2] B. Gustavsen, "Improving the pole relocating properties of vector
    fitting", IEEE Trans. Power Delivery, vol. 21, no. 3, pp. 1587-1592,
    July 2006.


Credits go to Bjorn Gustavsen for his MATLAB implementation.
(https://www.sintef.no/projectweb/vectorfitting/)
