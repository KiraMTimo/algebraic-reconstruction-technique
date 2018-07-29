# algebraic-reconstruction-technique

## Reference
Algebraic Reconstruction Technique (ART)
- https://en.wikipedia.org/wiki/Algebraic_reconstruction_technique

## Algebraic Reconstruction Technique (ART)
![asdf](https://en.wikipedia.org/wiki/File:Algebraic_Reconstruction_Technique_-_animated.gif)

        x^(k+1) = x^(k) + lambda_(k) * AT( y - A( x ) ) / AT( A( ones(size(x)) ) )

### 2) Shift in Spatial domain
f(x - a) <== Fourier Transform ==> exp(-j*2pi*a*kx) * FFT(f(x))

### 3) Shift in Fourier domain
exp(j*2pi*a*x) * f(x) <== Fourier Transform ==> FFT(f(x))(kx - a)

### 4) 1D Convolution theorem
(f*g)(x) <== Fourier Transform ==> FFT(f(x)) .* FFT(g(x))

where, * is convolution operator and .* is element-wise multiplication.

### 5) 2D Convolution theorem
(f*g)(x) <== Fourier Transform ==> FFT(f(x)) .* FFT(g(x))

where, * is convolution operator and .* is element-wise multiplication.
