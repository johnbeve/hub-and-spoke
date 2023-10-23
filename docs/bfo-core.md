The theory underwriting BFO is described in documentation such as "Building Ontologies with Basic Formal Ontology" and [ISO 21838:2](https://www.iso.org/standard/74572.html). 

The BFO theory is implemented in a handful of distinct formal languages, such as: 

* Common Logic Interchange Format (CLIF)
* First-Order Logic (FOL)
* Prover9 Syntax (Library for Automated Deduction Research)
* Web Ontology Language (OWL)

Most users of BFO employ the OWL implementation.

BFO is a weak formal theory in the sense that it can be logically extended in various ways; this is a feature, not a bug. 

A minimal OWL implementation of BFO was created that satisfies the ISO 21838:2 requirements, while also providing flexibility with respect to ontological modeling. 

This implementation is called "BFO-Core" and is found in the bfo-core.owl file. 

BFO-Core is comprised of all classes and relations identified in ISO 21838:2. 

Relations in BFO-Core are given a minimal temporal interpretation, namely, as holding at some time. For example, continuant_part_of(arm, Jake) is interpreted as "Arm is continuant part of Jake at some time". Consequently, object properties in BFO-Core do not exhibit role constraints, but only domain and range restrictions. It is in this sense that they exhibit minimal temporal interpretations. 
