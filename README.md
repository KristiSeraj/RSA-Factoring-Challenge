# RSA Factoring challenge

- [tests](https://github.com/KristiSeraj/RSA-Factoring-Challenge/tree/main/tests) - Test files for RSA factoring challenge

- [factors](https://github.com/KristiSeraj/RSA-Factoring-Challenge/blob/main/factors) - Factorize as many numbers as possible into a product of two smaller numbers
   - Usage: `factors <file>`
     - where `file` is a file containing natural numbers to factor.
     - One number per line
     - All lines will be valid natural numbers greater than 1
     - There will be no empty line, and no space before and after the valid number
     - The file will always end with a new line
   - Output format: `n=p*q`
     - one factorization per line
     - `p` and `q` don’t have to be prime numbers

**Example**:
```
root$ ./factors tests/test00
4=2*2
12=6*2
34=17*2
128=64*2
1024=512*2
4958=2479*2
1718944270642558716715=343788854128511743343*5
9=3*3
99=33*3
999=333*3
9999=3333*3
9797973=3265991*3
49=7*7
239809320265259=15485783*15485773
```

- [rsa](https://github.com/KristiSeraj/RSA-Factoring-Challenge/blob/main/rsa) - The same as `factors` but `p` and `q` are always prime numbers

**Example**:
```
root$ ./rsa tests/rsa-1
6=3*2
root$ ./rsa tests/rsa-2
77=11*7
root$ ./rsa tests/rsa-15
239821585064027=15486481*15485867
