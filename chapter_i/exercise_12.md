## Exercise 1.2 {#exercise-1-2}

Consider these documents:

Doc 1 breakthrough drug for schizophrenia

Doc 2 new schizophrenia drug

Doc 3 new approach for treatment of schizophrenia

Doc 4 new hopes for schizophrenia patients

Question:

1.  Draw the term-document incidence matrix for this document collection.

2.  Draw the inverted index representation for this collection, as in Figure 1.3 (page 7).

Answer:

1.  Term document incidence

| Term/Document | Doc 1 | Doc 2 | Doc 3 | Doc 4 |
| --- | --- | --- | --- | --- |
| approach | 0 | 0 | 1 | 0 |
| breakthrough | 1 | 0 | 0 | 0 |
| drug | 1 | 1 | 0 | 0 |
| hope | 0 | 0 | 0 | 1 |
| new | 0 | 1 | 1 | 1 |
| patient | 0 | 0 | 0 | 1 |
| schizophrenia | 1 | 1 | 1 | 1 |
| treatment | 0 | 0 | 1 | 0 |

1.  Inverted index

| approach | 3 |  |  |  |
| --- | --- | --- | --- | --- |
| breakthrough | 1 |  |  |  |
| drug | 1 | 2 |  |  |
| hope | 4 |  |  |  |
| new | 2 | 3 | 4 |  |
| patient | 4 |  |  |  |
| schizophrenia | 1 | 2 | 3 | 4 |
| treatment | 3 |  |  |  |