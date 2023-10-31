BFO adopts the following fundamental categories:
- universal and particular – Particulars are individual denizens of reality restricted to specific times and places, which instantiate universals, but which cannot be instantiated. Universals are repeatable across time and space and may have an indefinite number of instantiated particulars.
- continuant and occurrent – BFO is largely bifurcated into disjoint uni- versals5, distinguished by how particulars relate to time. Continuants endure through time maintaining identity, have no temporal parts, and are fully-present at any time they exist. Examples include house cats, the color of an apple, the function of mitochondria. By contrast, occurrent entities unfold over time or have temporal parts. Examples include: the history of Japan, drinking a cup of coffee, the temporal interval on which a mitotic division occurs.
- relations – BFO adopts three basic relation types: universal-universal, universal-particular, and particular-particular, the latter two of which may be time indexed. Universal-universal relations in BFO relate sub- types to parent types, whereas the sole universal-particular relation is the instance of relation, which holds between particulars and the univer- sals under which they fall.

There is often a practical need to accommodate terms in scientific discourse that do not correspond to universals. Examples of such terms include ‘medical doctor’ and disjunctions such as ‘dog or cat’. Such classes are called ‘defined classes’, and are represented as equivalent to any member satisfying a set of assertions whose non-logical symbols are satisfied by models consisting only of relations, universals, or instances of universals. In this way, we hold that ‘medical doctor’ is only a short-hand way of referring to instances of persons who bear a medical doctor role, and to be a ‘dog or cat’ is nothing over and above being an instance of dog or an instance of cat. As with the familiar notion of ‘defined class’ in the OWL2 specification, every defined class is rep- resented with an equivalency axiom, however, the ontological interpretation of the notion of asserted class as corresponding to a universal and ‘defined class’ as picking out a mere term is unique to BFO.


### Design Principles

## Monohierarchy Principle

Any class in any BFO-conformant ontology should - to the extent possible - have at most one asserted **is a** relation linking it to a parent class. This principle supports a simple strategy for formulating definitions and ontology taxonomies that avoids common errors in development.

Importantly, this principle applies to asserted ontology hierarchies and does not extend to inferred ontology hierarchies that may be generated using, for example, OWL reasoners. 

## Role Paraphrase Principle

Certain **independent continuants** such as pharmacists, lawyers, students, etc. are plausibly defined in terms of **roles** which instances bear. For example, a pharmacist just is an agent bearing a pharamcist role. 