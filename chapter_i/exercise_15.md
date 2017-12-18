## Exercise 1.5 {#exercise-1-5}

Extend the postings merge algorithm to arbitrary Boolean query formulas. What is its time complexity? For instance, consider:

1.  (Brutus OR Caesar) AND NOT (Antony OR Cleopatra)

Can we always merge in linear time? Linear in what? Can we do better than this?

Answer:

1.  Yes, we can always merge in linear time as input size going to be bigger since we need to find any postings which matched with any member in merged result of (Brutus OR Caesar), but not match in any posting inboth Antony AND Cleopatra. We can do better, by only take scan on postings which not included in merge result of (Brutus OR Caesar) and hope the merge result of (Brutus OR Caesar) always long.