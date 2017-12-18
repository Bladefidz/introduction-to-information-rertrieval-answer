## Exercise 1.7 {#exercise-1-7}

Recommend a query processing order for

1.  (tangerine OR trees) AND (marmalade OR skies) AND (kaleidoscope OR eyes)

given the following postings list sizes:

| Term | Postings Size |
| --- | --- |
| eyes | 213312 |
| kaleidoscope | 87009 |
| marmalade | 107913 |
| skies | 271658 |
| tangerine | 46653 |
| trees | 316812 |

Answer:

N(tangerine) + N(trees) = 363465

N(marmalade) + N(skies) = 379571

N(kaleidoscope) + N(eyes) = 1083321

Initial query is already omptimum.

(tangerine OR trees) AND (marmalade OR skies) AND (kaleidoscope OR eyes)