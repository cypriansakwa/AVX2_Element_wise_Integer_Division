This project shows how to use Rust's AVX2 instructions to perform element-wise integer division. 
Because AVX2 lacks direct support for integer division, this example requires floating-point conversion to complete the division.

## Overview
1. The function avx2_div performs element-wise division of two __m256i vectors.
    Because AVX2 does not directly allow integer division, the function converts the vectors to floating-point values, divides them, and then converts the results back to integer.

   ### Notes
   1.  This code is a simplistic example that has not been optimized for performance.
      In a production context, consider employing advanced AVX2 division algorithms or alternate integer division methods.
2. Check that your CPU supports AVX2 instructions, or you may need to alter the code or compilation settings accordingly.

   git clone https://github.com/cypriansakwa/AVX2_Element_wise_Integer_Division.git
   cd AVX2_Element_wise_Integer_Division
