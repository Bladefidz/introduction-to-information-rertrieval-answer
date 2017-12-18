## Exercise 1.4 {#exercise-1-4}

For the query below, can we still run through the intersection in time O(x+y), where x and y are the lengths of the postings lists for Brutus and Caesar? If not, what can we achieve?

1.  Brutus AND NOT Caesar

2.  Brutus OR NOT Caesar

answer

1.  Yes, we can still run O(x+y) as long as any postings of Caesar which matched with postings of Brutus is not intersected. Or in other, the length of intersected posting list is less than or equal to length of postings of Brutus.

2.  No, we can not achieve O(x+y) in x OR NOT y operation, since the length of NOT y is unknown and same as length of intersect posting list. We can optimize this query into O[x+y’], where y’ is length of postings which not existed in x and y.