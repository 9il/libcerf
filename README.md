libcerf
=======

Self-contained numeric library that provides an efficient and accurate implementation of complex error functions, along with Dawson, Faddeeva, and Voigt functions.

####Functions:
* fadeeva (complex)
* erfcx (both)
* erfi (both)
* dawson (both)
* voigt
* erf (complex)
* erfc (complex)


####Example:
```D
import std.complex, std.math;
import libcerf;

auto c = erfi(complex(1.0, 0.0));
auto f = erfi(1.0);

assert(fabs((c.re - f)/f) < 1e-13);
```

####Links
* D source code at [GitHub](http://github.com/9il/libcerf)
* Original [Faddeeva Package](http://ab-initio.mit.edu/wiki/index.php/Faddeeva_Package)
* Original C [source code](http://github.com/9il/libcerf)