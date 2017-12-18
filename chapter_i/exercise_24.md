## Exercise 2.4 {#exercise-2-4}

For the Porter stemmer rule group shown in (2.1):

1.  What is the purpose of including an identity rule such as SS → SS?

    To identify such term belong to adjective.

2.  Applying just this rule group, what will the following words be stemmed to?

    circus canaries boss

    circuscanari boss

3.  What rule should be added to correctly stem _pony_?

    IESS → Y

4.  The stemming for _ponies_ and _pony_ might seem strange. Does it have a deleterious effect on retrieval? Why or why not?

    No, it does not have high deleterious effect on retrieval result because _poni_ as result of stemming of _ponies_ and _pony_have been stored at index at first will always matched with _poni_ from post processed term of query.