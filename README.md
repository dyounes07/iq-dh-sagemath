# IQ-DH Demonstration

A SageMath implementation demonstrating a toy Diffie–Hellman-style key exchange
using the ideal class group of an imaginary quadratic field.

## Overview

Two parties choose private random exponents and use a public generator from an
ideal class group to derive public values. Each party then exponentiates the
other party's public value using their own private exponent.

The resulting shared ideal classes should be equal:

```text
(public_B)^a = (public_A)^b
