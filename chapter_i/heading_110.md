## Heading 1.10 {#heading-1-10}

Write out a postings merge algorithm, in the style of Figure 1.6 (page 11), for an x OR y query.

Answer:

INVERTED_INDEX *px = x

INVERTED_INDEX *py = y

INVERTED_INDEX *z = allocate()

while (*px).next != null || (*py).next != null:

if (*px).docId != null &amp;&amp; (*py).docId != null:

if (*px).docId == (*py).docId:

(*z).docId = (*px).docId

px = (*px).next

py = (*py).next

else:

if px.docId &lt; py.doId:

(*z).docId = (*px).docId

px = (*px).next

else:

(*z).docId = (*py).docId

py = (*py).next

else:

if px != null:

(*z).docId = (*px).docId

else:

(*z).docId = (*py).docId

(*z).next = alocate()

z = (*z).next

&amp;z = null