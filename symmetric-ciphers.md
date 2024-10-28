
# Symmetric Ciphers

## One Time Pad

XOR random bit-string of length $l$ - the pad - with a message of length $l$. This is a one-time pad.

$P = \\{0 | 1\\}^l$

$M = \\{0 | 1\\}^l$

$C = P \oplus M$

$P$ cannot be reused. Reason:

$P = \\{0 | 1\\}^l$

$C1 = P \oplus M1$

$C2 = P \oplus M2$

$C1 \oplus C2 = (M1 \oplus P) \oplus (M2 \oplus P) = M1 \oplus M2$ - if the messages are structured you can recover the plaintexts.

## Symmetric Cipher

