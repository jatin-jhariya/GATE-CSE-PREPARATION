# NUMBER SYSTEM — GATE REVISION

## 1. DIVISIBILITY

**2** → Last digit even
**3** → Sum of digits divisible by 3
**4** → Last 2 digits divisible by 4
**5** → Last digit 0/5
**6** → Divisible by 2 & 3
**8** → Last 3 digits divisible by 8
**9** → Sum of digits divisible by 9
**11** → Difference of alternate digit sums divisible by 11

---

## 2. PRIME FACTORIZATION

If

`N = p₁^a₁ × p₂^a₂ × ... × pₖ^aₖ`

### Number of factors

`d(N) = (a₁+1)(a₂+1)...(aₖ+1)`

### Sum of factors

`σ(N) = [(p₁^(a₁+1)-1)/(p₁-1)] × ...`

### Perfect Square

All `aᵢ` = **even**

### Perfect Cube

All `aᵢ` = **multiples of 3**

---

## 3. HCF & LCM

For prime powers:

**HCF** → minimum exponent

**LCM** → maximum exponent

For two positive integers:

`HCF × LCM = Product`

If `gcd(a,b)=1`:

`LCM(a,b)=ab`

---

## 4. NUMBER OF FACTORS — IMPORTANT CASES

If `N = p^a`

`d(N)=a+1`

If `N = p^a q^b`

`d(N)=(a+1)(b+1)`

### Odd factors

Ignore factor 2.

### Even factors

`Total factors − Odd factors`

### Perfect-square factors

For `N = p₁^a₁...pₖ^aₖ`

`# square divisors = (⌊a₁/2⌋+1)...(⌊aₖ/2⌋+1)`

---

## 5. REMAINDER

`Dividend = Divisor × Quotient + Remainder`

`0 ≤ R < Divisor`

### Properties

`(a+b) mod m = [(a mod m)+(b mod m)] mod m`

`(a−b) mod m = [(a mod m)−(b mod m)] mod m`

`ab mod m = [(a mod m)(b mod m)] mod m`

---

## 6. MODULAR ARITHMETIC

`a ≡ b (mod m)`
⟺ `m | (a−b)`

If:

`a ≡ b (mod m)`

then

`a^n ≡ b^n (mod m)`

### Negative remainder

If `a mod m = r`

`(-a) mod m = m-r`

---

## 7. CYCLICITY

For `a^n mod m`:

**Step 1:** Find cycle
**Step 2:** Find cycle length `k`
**Step 3:** Calculate `n mod k`

If remainder = 0 → take **last term of cycle**

### Common cycles

`2 → 2,4,8,6` → length 4

`3 → 3,9,7,1` → length 4

`4 → 4,6` → length 2

`7 → 7,9,3,1` → length 4

`8 → 8,4,2,6` → length 4

`9 → 9,1` → length 2

---

## 8. UNIT DIGIT

Only the **last digit** matters.

For `a^n`:

Reduce base to last digit → find cycle → use exponent.

**Special:**

`0^n → 0`

`1^n → 1`

`5^n → 5`

`6^n → 6`

`n > 0`

---

## 9. FACTORIAL

`n! = n(n−1)...2×1`

`0! = 1`

### Highest power of p dividing n!

`vₚ(n!) = ⌊n/p⌋ + ⌊n/p²⌋ + ⌊n/p³⌋ + ...`

---

## 10. TRAILING ZEROES

For `n!`:

`Z = ⌊n/5⌋ + ⌊n/25⌋ + ⌊n/125⌋ + ...`

**Reason:** 10 = 2×5 and factors of 2 are more abundant.

---

## 11. LAST DIGITS

For last `k` digits:

Find

`N mod 10^k`

Examples:

Last digit → mod 10
Last 2 digits → mod 100
Last 3 digits → mod 1000

---

## 12. NUMBER OF DIGITS

For `N > 0`:

`Number of digits = ⌊log₁₀N⌋ + 1`

For `a^n`:

`Digits = ⌊n log₁₀a⌋ + 1`

---

## 13. DIVISIBILITY OF POWERS

If `a` and `m` are coprime:

Use **Euler's theorem**:

`a^φ(m) ≡ 1 (mod m)`

### Fermat's Little Theorem

If `p` is prime and `gcd(a,p)=1`:

`a^(p−1) ≡ 1 (mod p)`

---

## 14. EULER PHI FUNCTION

`φ(n)` = numbers ≤ n that are coprime to n.

If `p` is prime:

`φ(p)=p−1`

If `n=p^k`:

`φ(p^k)=p^k−p^(k−1)`

General:

`φ(n)=n ∏(1−1/p)`

where p = distinct prime factors of n.

---

# GATE TRAPS ⚠️

* `1` → neither prime nor composite
* `2` → only even prime
* Remainder is always `< divisor`
* `0! = 1`
* For unit digit → **cycle**, not direct calculation
* For trailing zeroes → count **5**, not 10
* HCF → **minimum powers**
* LCM → **maximum powers**
* Last `k` digits → **mod 10^k**
* Perfect square → every exponent **even**
* Perfect cube → every exponent **multiple of 3**
