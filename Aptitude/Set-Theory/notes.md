## 1. BASIC SET FORMULAS

* \(A\cup B\): Union
* \(A\cap B\): Intersection
* \(A-B=A\cap B'\)
* \(A'\): Complement of A
* \(A\cap B=\varnothing\): Disjoint sets

**De Morgan's Laws**

* \((A\cup B)'=A'\cap B'\)
* \((A\cap B)'=A'\cup B'\)

## 2. CARDINALITY FORMULAS

**Two sets:**

$$
|A\cup B|=|A|+|B|-|A\cap B|
$$

Neither A nor B:

$$
N-|A\cup B|
$$

Only A:

$$
|A|-|A\cap B|
$$

Exactly one:

$$
|A|+|B|-2|A\cap B|
$$

**Three sets:**

$$
\begin{aligned}
|A\cup B\cup C|={}&|A|+|B|+|C|\\
&-|A\cap B|-|B\cap C|\\
&-|C\cap A|+|A\cap B\cap C|
\end{aligned}
$$

None of the three:

$$
N-|A\cup B\cup C|
$$

Only A:

$$
|A|-|A\cap B|-|A\cap C|+|A\cap B\cap C|
$$

Exactly two:

$$
|A\cap B|+|B\cap C|+|C\cap A|-3|A\cap B\cap C|
$$

At least two:

$$
|A\cap B|+|B\cap C|+|C\cap A|-2|A\cap B\cap C|
$$

## 3. VENN DIAGRAM SHORTCUTS

* **At least one** = Union
* **Neither** = Total − At least one
* **Only A** = A − all overlapping regions
* **Exactly one** = Only A + Only B (+ Only C)
* **Exactly two** = Pairwise intersections excluding the triple intersection
* **At least two** = Exactly two + Exactly three

**3-set solving order:**

1. Fill the centre \(A\cap B\cap C\).
2. Fill pairwise-only regions.
3. Fill individual-only regions.
4. Calculate outside region.

⚠️ If pairwise intersection values include the centre, subtract the centre to obtain pairwise-only values.

## 4. USEFUL IDENTITIES

$$
|A-B|=|A|-|A\cap B|
$$

$$
|A\triangle B|=|A|+|B|-2|A\cap B|
$$

$$
|A'|=N-|A|
$$

If \(A\subseteq B\):

$$
A\cap B=A,\qquad A\cup B=B
$$

## 5. GATE QUESTION PATTERNS

* Two-set / three-set inclusion–exclusion
* Only / exactly / at least / neither
* Students knowing different subjects or languages
* Survey questions involving overlapping groups
* Find missing intersection or total population
* Verify whether given set counts are possible

## QUICK REMINDERS

**Union → Add individual sets, subtract pairwise intersections, add triple intersection.**

**Neither → Total − Union.**

**Exactly two (3 sets) → Pairwise sum − 3 × triple intersection.**

**At least two (3 sets) → Pairwise sum − 2 × triple intersection.**
