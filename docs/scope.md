# Scope

A long-standing issue among BFO users and developers has concerned how best to represent time. Importantly, issues concerning time in BFO stem from implementations of BFO in restricted formal languages such as OWL. OWL does not allow for direct representation of relations with arity higher than two. To illustrate the issue, consider modeling a vehicle having an engine part at some time, but losing that engine part at another. An expressive language such as First-Order Logic (FOL) would permit the following representation: 

    has_part(vehicle, engine, time_1) & ~has_part(vehicle, engine, time_2)

Since FOL allows using ternary relations. OWL's restriction to at most binary relations precludes expressions like (1); indeed, there is no simple, straightforward way
to represent the content of (1) in OWL. Given the need to represent time and change in many domains and the wide use of OWL in ontology circles, there have been numerous proposals by users of BFO for representing such phenomena within the binary constraints of OWL, each with limited success.

## BFO-Core

To avoid imposing unnecessarily restrictive temporal commitments on users of BFO, an OWL representation of BFO having minimal temporal semantics was created - known as **BFO-Core**. Motivations for creating such a core include:

> 1. Scientific domains do not treat time uniformly. Economists, for example, measure economic constructs using time series, i.e. presuming a model of discrete time, whereas physicists typically treat time as continuous. This observation speaks in favor of BFO remaining neutral on questions over the discreteness of continuity of time. 
> 2. Not all scientific domains require a robust characterization of time, e.g. the domain of mathematics has no obvious need for time. 
> 3. Given community goals, even if users need some characterization of time, they do not always need a robust characterization of time, e.g. [Open Biological and Biomedical Ontology Foundry](https://obofoundry.org/) users have, for many years, employed a formally weak representation of time with great success.
    
This last point is worth belaboring. Deploying a BFO-based, robust, formalization of time can be costly, involving re-educating users, updating existing ontologies, perhaps even rewriting portios of codebases, etc. OBO users have not often had a need for such rigor, and so do not have a need to bear such costs. A charitable reading of early [criticisms](https://github.com/cmungall/trel-crit/raw/master/trc.pdf) of the Temporalized Relations strategy - which provides a rather robust formalization of time in BFO - makes just this point.  

On the other hand, there are reasons that speak in favor of providing formal guidance for modeling time in BFO:

> 4. Other foundry efforts, such as the [Industrial Ontology Foundry](https://www.industrialontologies.org/) which uses BFO as its top-level architecture, anticipate the need for a rigorous formalization of time.
> 5. [Recent work](https://pubmed.ncbi.nlm.nih.gov/36534832/) demonstrating the importance of rigorous axiomatization of ontologies used to supplement machine learning pipelines with minimal datasets, suggests rigorous BFO formalizations of time ontologies may be useful in such contexts. 

What these observations suggest is that while there are strong motivations for BFO providing - perhaps significant - guidance to users who require a robust formalization of time, imposing any specific formalization of time on all users would be in some cases unnecessarily onerous. 

To satisfy needs of the community then, the BFO development team encourages a strategy of developing and deploying **Temporal Extensions** of **BFO-Core** which will provide users options for representing time in their domains. In what follows, we discuss **BFO-Core** and the **Temporalized Relations** extension of the core.