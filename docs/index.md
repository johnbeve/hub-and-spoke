# Basic Formal Ontology 

## Forward
  This is a user guide meant for...OWL users

The World Wide Web Consortium [W3C](https://www.w3.org/) describes a collection of standards and technologies that facilitate information sharing and reuse across applications and the web. Key standards for ontology and knowledge graph engineering include the Resource Description Framework [RDF](https://www.w3.org/TR/rdf11-concepts/), the Resource Description Framework Schema [RDFS](https://www.w3.org/TR/rdf-schema/), the OWL Web Ontology Language [OWL2](https://www.w3.org/TR/owl2-overview/) and the SPARQL Protocol and RDF Query Language [SPARQL](https://www.w3.org/TR/sparql11-query/).

### RDF
The Resource Description Framework (RDF) is a framework for representing information in the Web. RDF graphs are sets of subject-predicate-object triples, where the elements may be IRIs, blank nodes, or datatyped literals. They are used to express descriptions of resources. [RDF](https://www.w3.org/TR/rdf11-concepts/)

### RDFS
RDF Schema provides a data-modelling vocabulary for RDF data. RDF Schema is an extension of the basic RDF vocabulary. [RDFS](https://www.w3.org/2001/sw/wiki/RDFS) 

### OWL
The OWL 2 Web Ontology Language, informally OWL 2, is an ontology language for the Semantic Web with formally defined meaning. OWL 2 ontologies provide classes, properties, individuals, and data values and are stored as Semantic Web documents. OWL 2 ontologies can be used along with information written in RDF, and OWL 2 ontologies themselves are primarily exchanged as RDF documents. [OWL2](https://www.w3.org/TR/owl2-overview/)

### Domain

The domain of BFO is comprised of particulars or instances that stand in the primitive **instances of** relation to universals at times. BFO’s hierarchy of universals can be represented by defining the relation:

    ∀(x,t) is_a(A,B)=<sub>def</sub> instance_of(x,A,t) → instance_of(x,B,t)

For example, material entity is a independent continuant.

Nearly all classes in BFO are **rigid** which means that is an instance is a member of such a class, then it is a member of that class for as long as the instance exists. For example, we say the class continuant is rigid since any given instance of continuant remains an instance of continuant as long as it exists. There are three classes in BFO that are not rigid: fiat object part, object, and object aggregate. For example, an instance of object aggregate may at some later time be an instance of the class object.
