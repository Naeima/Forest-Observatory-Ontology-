# Forest Observatory Ontology 

The Forest Observatory Ontology (FOO) ( is an ontology for describing wildlife data generated by sensors. FOO's scope evolves around the Internet of Things (IoT) and wildlife habitats. To illustrate our datasets of interest, we modelled the concept to represent "sensors observing animals and land". These sensors generate observations. For example, the animal GPS collar tracks an elephant and records its geo-location observations for different and equally spaced time intervals and temperature every specified time interval. We adopted classes and properties from SOSA [11] and BBC wildlife [1] ontologies to model the domain coverage.



![image](https://user-images.githubusercontent.com/57564713/185769396-6a963789-43da-4993-9273-cf2c37256595.png)




# FOO specification draft
https://github.com/Naeima/Forest-Observatory-Ontology-/releases/download/v1.0.0/index-en.html


# OOPS! (OntOlogy Pitfall Scanner!) results
https://github.com/Naeima/Forest-Observatory-Ontology-/releases/download/v1.0.0/oopsEval.html


# FOO Development

We developed FOO following the Linked Open Terms (LOT) [6] methodology using a complied list of comptency questions (functional requirements)- implemented in protege software.  LOT  was originated from Neon methodology, it encourages borrowing and reusing classes from fully developed and widely shared ontologies. Therefore, we searched the existing literature for suitable ontologies. Then, we decided to borrow classes and relationships from SOSA and BBC Wildlife Ontologies, as they contained sufficient components to model our proposed entities (i.e., instances or individuals). Moreover, LOT recommends sharing ontologies according to the Linked Data principles to enable re-using the ontologies by the research community and software applications. 

<img width="1305" alt="FOOSensor" src="https://user-images.githubusercontent.com/57564713/187103336-263758f5-ba32-439f-b9c1-836569f02526.png">








# Repository

This repository has a copy of the following:

•	Ontology Requirements Specification Document (ORSD).

•	A spreadsheet contains the ontology functional requirements (i.e., comptency questions). 

•	Ontology in RDF/XML and TURTLE formats.

•	Ontology documentation using WIDOCO tool

•	Soil data properties across primary forest, logged forest and oil palm plantation in Sabah, Malaysia [9] [12].


# SPARQL Query example 
What objects do contain the word sensor? 

    PREFIX rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#>.

    PREFIX owl: <http://www.w3.org/2002/07/owl#>.

    PREFIX rdfs: <http://www.w3.org/2000/01/rdf-schema#>.

    PREFIX xsd: <http://www.w3.org/2001/XMLSchema#>.


    SELECT ?subject ?predicate ?object

    WHERE { ?subject ?predicate  ?object.
    
    FILTER REGEX(?object, ("Sensor"))}
    

![sensor](https://user-images.githubusercontent.com/57564713/185769348-497951cf-6b9d-465b-98f8-8a67b99121df.png)


![Stardog](https://user-images.githubusercontent.com/57564713/187270662-9236804f-3e1c-4425-a8c1-535e2a96776e.png)

# Instantiating FOO with dataset about soil properties.

https://github.com/Naeima/Forest-Observatory-Ontology/releases/tag/Soil-Data-v1.0.0

![soil](https://user-images.githubusercontent.com/57564713/186782688-5561c88d-09d5-4b37-990a-fe290b91fe60.png)


# How to use FOO

https://github.com/Naeima/Forest-Observatory-Ontology/releases/tag/How-to-run-FOO-v1.0.0



# References

[1] 2022.  https://www.bbc.co.uk/ontologies/wildlife

[2] Daniel Garijo. 2017. WIDOCO: a wizard for documenting ontologies. In International Semantic Web Conference. Springer,
94–102. https://dgarijo.github.io/Widoco/

[3] 2022. OOPS! - OntOlogy Pitfall Scanner! https://oops.linkeddata.es/

[4] 2022. Protégé. https://protege.stanford.edu/

[5] 2022. Semantic Sensor Network Ontology.https://www.w3.org/TR/vocab-ssn/

[6] María Poveda-Villalón, Alba Fernández-Izquierdo, Mariano Fernández-López, and Raúl García Castro. 2022. LOT:An industrial oriented ontology engineering framework. Engineering Applications of Artificial Intelligence 111 (2022), 104755.https://www.sciencedirect.com/science/article/pii/S0952197622000525

[7] Asunción Gómez-Pérez and Mari Carmen Suárez-Figueroa. 2009. NeOn methodology for building ontology networks:a scenario-based methodology (2009), https://oa.upm.es/5475/1/INVE_MEM_2009_64399.pdf

[8] Milena Salgado Lynn and Amaziasizamoria Jumail. 2021. The Danau Girang Field Centre: Field Station Profile.ECOTROPICA 23, 1/2 (2021), 202103–202103. https://www.ecotropica.eu/index.php/ecotropica/article/view/86/26

[9] Elias et. al. 2018. Soil properties across primary forest, logged forest and oil palm plantation in Sabah, Malaysia.
https://doi.org/10.5285/7e046092-8405-41b8-9e38-67a844bb9e7d.

[10] Mari Carmen Suárez-Figueroa, Asunción Gómez-Pérez, and Boris Villazón-Terrazas. 2009. How to write and use
the ontology requirements specification document. In OTM Confederated International Conferences" On the Move to
Meaningful Internet Systems". Springer, 966–982.

[11] Krzysztof Janowicz, Armin Haller, Simon J.D. Cox, Danh Le Phuoc, and Maxime Lefrançois. 2019. 
SOSA: A lightweight ontology for sensors, observations, samples, and actuators. Journal of Web Semantics 56, (2019), 1–10. DOI: https://doi.org/10.1016/j.websem.2018.06.003

[12] Soil properties across primary forest, logged forest and oil palm plantation in Sabah, Malaysia - data.gov.uk. Retrieved January 21, 2022 from https://data.gov.uk/dataset/e54d035f-4bcb-4d65-a600-043a2c0f729a/soil-properties-across-primary-forest-logged-forest-and-oil-palm-plantation-in-sabah-malaysia




