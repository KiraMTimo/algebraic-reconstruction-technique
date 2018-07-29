# algebraic-reconstruction-technique

## Reference
Algebraic Reconstruction Technique (ART)
- https://en.wikipedia.org/wiki/Algebraic_reconstruction_technique

## Algebraic Reconstruction Technique (ART)
The `algebraic reconstruction technique (ART)` is a class of iterative algorithms used in computed tomography. 

An advantage of ART over other reconstruction methods ( such as `filtered backprojection (FBP)` which is deterministic method ) is that it is relatively easy to incorporate prior knowledge into the reconstruction process.

        x^(k+1) = x^(k) + lambda_(k) * AT( y - A( x ) ) / AT( A( ones(size(x)) ) )
        
        where,  A() is radon transform ( called by projection ) 
        
                AT() is inverse radon transform without filtration ( called by backprojection ).
