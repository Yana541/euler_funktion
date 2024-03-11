# Euler's Totient Function

## Description

### Definition

Euler's totient function `phi(n)` (sometimes denoted as `varphi(n)` or `phi(n)` is the number of positive integers less than or equal to `n` that are coprime to ` n`. In other words, it is the count of integers in the range `[1, n]` whose greatest common divisor with ` n ` is 1.

The first few values of this function (A000010 in the OEIS) are:

`phi(1)` = 1
`phi(2)` = 1 
`phi(3)`= 2
`phi(4)` = 2 
`phi(5)` = 4 

### Properties

Three fundamental properties of Euler's totient function are sufficient to compute it for any given number:

1. If `p ` is a prime number, then `phi(p) = p - 1 `
    - (This is obvious because any number other than `p` is coprime with ` p `).

2. If ` p ` is a prime and ` a ` is a positive integer, then `phi(p^a) = p^a - p^a-1`.
    - (Since the only numbers not coprime with  `p^a` are multiples of `p`, there are `p^a / p = p^a-1` such multiples.)

3. If `a ` and `b` are coprime, then `phi(ab) = phi(a) * phi(b) ` (Euler's totient function is "multiplicative").
    - (This fact follows from the Chinese remainder theorem. Consider an arbitrary number  `z ≤ ab `. Let `x` and `y` be the remainders when zz is divided by aa and bb respectively. Then `z` is coprime with `ab` if and only if `z` is coprime with both `a` and `b` individually, or equivalently, `x` is coprime with  `a` and `y` is coprime with `b`. Applying the Chinese remainder theorem yields the unique correspondence between any pair of numbers `x` and `y` (`x≤a`, `y≤b`) and a number `z` `(z≤ab)`, completing the proof.)
From these properties, Euler's totient function for any `n` can be derived through its factorization (decomposition of ` n` into prime factors):

If

![изображение](https://github.com/Yana541/euler_funktion/assets/149325426/286a57a5-4ed2-48ba-9bc4-fb5eab72b4f3)


(where all `p_i` are prime), then

![изображение](https://github.com/Yana541/euler_funktion/assets/149325426/b7bb0580-a673-425a-9f3f-6dd3e0b2861a)
