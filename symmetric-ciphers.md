
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

This works because given an $M$ bit and a $P$ bit, $P(M \oplus P = 0) = P(M \oplus P = 1) = 0.5$. 

## Symmetric Cipher

- We want the properties of a one-time pad and the following additional properties:
	- Fixed $P$ length independent of $M$ length.

This property is important because OTP management becomes painful to manage.

Symmetric Cipher ergonomics:

- Single Secret $K$ 
- Nonce $n$ that is unique per-message and not reused
- 
