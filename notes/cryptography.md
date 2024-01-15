- RSA
	1. choose 2 unique prime, p & q
	2. $n = p * q$ 
	3. $\phi(n) = (p-1) * (q-1)$ 
	4. $e =$ coprime of $\phi(n)$ 
	5. $ed =$ mod $\phi(n)$ 
	6. public key {e, n}, private key {d, n}
	7. CT = PT ^ e mod n, PT = CT ^ d mod n
