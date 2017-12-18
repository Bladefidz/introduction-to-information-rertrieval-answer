## Exercise 1.8 {#exercise-1-8}

If the query is:

1.  friends AND romans AND (NOT countrymen)

How could we use the frequency of countrymen in evaluating the best evaluation order? In particular, propose a way of handling negation in determining the order of query processing.

Answer:

The merge result from this query is any intersected term from friends AND romans that **not matched** with any terms found in countrymen. The result length should be smaller than or equal to the length of friend AND romans.