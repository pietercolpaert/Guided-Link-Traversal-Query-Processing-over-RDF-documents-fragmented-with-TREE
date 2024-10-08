# Exploring a rule-based approach for source selection in link traversal queries

## Abstract

Link Traversal queries face challenges in completeness and long execution time due to the size of the web.
Reachability criteria define completeness by restricting the links followed by engines. However, the number of
links to dereference remains the bottleneck of the approach. Web environments often have structures exploitable
by query engines to prune irrelevant sources. Current criteria rely on using information from the query definition
and predefined predicate. However, it is difficult to use them to traverse environments where logical expressions
indicate the location of resources. We propose to use a rule-based reachability criterion that captures logical
statements expressed in hypermedia descriptions within linked data documents to prune irrelevant sources. In
this poster paper, we show how the Comunica link traversal engine is modified to take hints from a hypermedia
control vocabulary, to prune irrelevant sources. Our preliminary findings show that by using this strategy, the
query engine can significantly reduce the number of HTTP requests and the query execution time without
sacrificing the completeness of results. Our work shows that the investigation of hypermedia controls in link
pruning of traversal queries is a worthy effort for optimizing web queries of unindexed decentralized databases.


## Building a PDF
The authors compiled the PDF version using `pdflatex` (you can use your favorite latex compiler).
We created a `makefile` to facilitate the building of the PDF version.
One can simply execute `make main.pdf` or `make` to produce the PDF version if `pdflatex` and the other dependencies of the [TeX Live](https://tug.org/texlive/) suite are installed on the machine of the user.


## Conclusion

The publication of linked data in SPARQL endpoints is not always a sustainable approach due to
unavailability and cost problems. Our work is centered around decentralized alternatives for linked data
publication. Our preliminary results show that our rule-based reachability criterion can significantly
reduce the execution time of queries aligned with hypermedia description constraints compared to
predicate-based reachability opening the possibility for faster and more versatile traversal-based query
execution over fragmented RDF documents. Our experiment also highlights that the size of the internal
data store might have more impact on performance than noted in previous studies. In future work, we
will perform more exhaustive evaluations of other types of domain-oriented fragmentation strategies
such as string evaluation and geospatial, and investigate how to generalize our approach to support
more expressive online reasoning for online source selection during traversal queries.

