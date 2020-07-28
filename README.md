# Hello chicken scheme

Playing around with [CHICKEN scheme][1].

## palindrome

```bash
csc -o palindrome palindrome.scm
./palindrome ANNA
```
Should output `ANNA is a palindrome`

## quickrep

```bash
csc quickrep.scm
csi -ss quickrep.scm <quickrep.dat 'a.*c' A
```
Should output:
```
xyzAghi
Agh
foonly
```

## fib (with C lib)
Example taken from https://api.call-cc.org/4/doc/chicken/intro#sec:Accessing_C_libraries_

```bash
gcc -c fib.c
csc -o fib-user fib.o fib-user.scm
./fib-user
```
Should output: `1 1 2 3 5 8 13 21 34 55 89`

[1]: https://call-cc.org/
