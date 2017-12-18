## Exercise 1.11 {#exercise-1-11}

How should the boolean query x AND NOT y be handled? Why is naive evaluation of this query normally very expensive? Write out a postings merge algorithm that evaluates this query efficiently.

Answer:

Find any terms of x that not matched with terms of y. The algorithm may be like this:

INVERTED_INDEX *px = x

INVERTED_INDEX *py = y

INVERTED_INDEX *z = allocate()

while px != null:

if (*px).docId &lt; (*py).docId:

(*z).docId = (*px).docId

px = (*px).next

else:

py = (*py).next

(*z).next = allocate()

z = (*z).next

&amp;z = null