# Temporal Extensions

Temporal extensions should be implemented in a decidable flavor of OWL, such as [OWL2-DL](https://www.w3.org/TR/owl2-overview/). While terminological content differs across temporal profiles, developers are encouraged to abide by the following design principles: 

- The scope of Temporal Extensions should include treatment of classes and relationships such as: 
    - Temporal Region and subclasses 
    - Spatiotemporal Region 
    - Object properties relating to time, whether explicit or implicit
    - Temporal Extension Artifacts should be represented in some serialization of RDF, e.g. ttl, owl.
    - Use, as a starting point, design patterns and use cases concerning time and change found in the article [Basic Formal Ontology: Case Studies](https://philpapers.org/archive/OTTBBF.pdf). There the authors present seven design patterns based on the FOL implementation of BFO. 

## Temporal Extension Integration

Putting aside the varying relative maturity levels of each Temporal Extension, there is a further pressing question concerning interoperability. BFO is a top-level ontology designed to provide a common hierarchy across all scientific research; interoperability is its motivation. With this in mind, it is thus incumbent on developers to demonstrate not only that their preferred formalization of time conforms to BFO, but also that interpretations, formal mappings, or provable containments exists across strategies. This is, admittedly, a great deal of work, but it is a consequence of sustaining interoperability, a goal our community prizes.

# Temporal Extensions Implementation


## Temporalized Relations Design Patterns


## Temporal Extension Further Reading
[Temporally Qualified Continuants](https://jansenludger.github.io/home/Texte/TQC%20Freiburg8%20Proceedings.pdf) \
[Temporal Snapshots](https://oborel.github.io/obo-relations/temporal-semantics/) 
