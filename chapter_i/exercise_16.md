## Exercise 1.6 {#exercise-1-6}

We can use distributive laws for AND and OR to rewrite queries.

1.  Show how to rewrite the query in Exercise 1.5 into disjunctive normal form using the distributive laws.

2.  Would the resulting query be more or less efficiently evaluated that the original form of this query?

3.  Is this result true in general or does it depend on the word and the contents of the document collection?

Answer

1.  
2.  Would be less efficiently because we need to produce each negation first before operation OR.

3.  It is true for general.