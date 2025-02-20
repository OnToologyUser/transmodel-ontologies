# Transmodel Ontology - Facilities

![OOPS!](http://vocab.linkeddata.es/ontologies/oops/logomini.png)

The following evaluation results have been generated by the [RESTFul web service](http://oops-ws.oeg-upm.net/) provided by [OOPS!](http://oops.linkeddata.es/) (OntOlogy Pitfall Scanner!).

It is obvious that not all the pitfalls are equally important; their impact in the ontology will depend on multiple factors. For this reason, each pitfall has an importance level attached indicating how important it is. We have identified three levels:


<img src="https://raw.githubusercontent.com/OnToology/oops-report/master/sample/critical.png" height="15px"> It is crucial to correct the pitfall. Otherwise, it could affect the ontology consistency, reasoning, applicability, etc.

<img src="https://raw.githubusercontent.com/OnToology/oops-report/master/sample/important.png" height="15px"> Though not critical for ontology function, it is important to correct this type of pitfall.

<img src="https://raw.githubusercontent.com/OnToology/oops-report/master/sample/minor.png" height="15px"> It is not really a problem, but by correcting it we will make the ontology nicer.



## Pitfalls



#### P04. Creating unconnected ontology elements <img src="https://raw.githubusercontent.com/OnToology/oops-report/master/sample/minor.png" height="15px"> (7 cases detected).
*Ontology elements (classes, object properties and datatype properties) are created isolated, with no relation to the rest of the ontology.*

    

#### P11. Missing domain or range in properties <img src="https://raw.githubusercontent.com/OnToology/oops-report/master/sample/important.png" height="15px"> (62 cases detected).
*Object and/or datatype properties without domain or range (or none of them) are included in the ontology.*

    

#### P13. Inverse relationships not explicitly declared <img src="https://raw.githubusercontent.com/OnToology/oops-report/master/sample/minor.png" height="15px"> (71 cases detected).
*This pitfall appears when any relationship (except for those that are defined as symmetric properties using owl:SymmetricProperty) does not have an inverse relationship (owl:inverseOf) defined within the ontology.*

    

#### SUGGESTION: symmetric or transitive object properties.. symmetric or transitive object properties. <img src="https://raw.githubusercontent.com/OnToology/oops-report/master/sample/minor.png" height="15px"> (1 cases detected).
*The domain and range axioms are equal for each of the following object properties. Could they be symmetric or transitive?*

    

#### P24. Using recursive definitions <img src="https://raw.githubusercontent.com/OnToology/oops-report/master/sample/important.png" height="15px"> (2 cases detected).
*An ontology element (a class, an object property or a datatype property) is used in its own definition. Some examples of this would be: (a) the definition of a class as the enumeration of several classes including itself;  (b) the appearance of a class within its owl:equivalentClass or rdfs:subClassOf axioms; (c) the appearance of an object property in its rdfs:domain or range rdfs:range definitions; or (d) the appearance of a datatype property in its rdfs:domain definition.*

    

#### P19. Defining multiple domains or ranges in properties <img src="https://raw.githubusercontent.com/OnToology/oops-report/master/sample/critical.png" height="15px"> (3 cases detected).
*The domain or range (or both) of a property (relationships and attributes) is defined by stating more than one rdfs:domain or rdfs:range statements. In OWL multiple rdfs:domain or rdfs:range axioms are allowed, but they are interpreted as conjunction, being, therefore, equivalent to the construct owl:intersectionOf. This pitfall is related to the common error that appears when defining domains and ranges described in [7].*

    

#### P21. Using a miscellaneous class <img src="https://raw.githubusercontent.com/OnToology/oops-report/master/sample/minor.png" height="15px"> (1 cases detected).
*This pitfall refers to the creation of a class with the only goal of classifying the instances that do not belong to any of its sibling classes (classes with which the miscellaneous problematic class shares a common direct ancestor).*

    

#### P02. Creating synonyms as classes <img src="https://raw.githubusercontent.com/OnToology/oops-report/master/sample/minor.png" height="15px"> (1 cases detected).
*Several classes whose identifiers are synonyms are created and defined as equivalent (owl:equivalentClass) in the same namespace. This pitfall is related to the guidelines presented in [2], which explain that synonyms for the same concept do not represent different classes.*

    

#### P08. Missing annotations <img src="https://raw.githubusercontent.com/OnToology/oops-report/master/sample/minor.png" height="15px"> (52 cases detected).
*This pitfall consists in creating an ontology element and failing to provide human readable annotations attached to it. Consequently, ontology elements lack annotation properties that label them (e.g. rdfs:label, lemon:LexicalEntry, skos:prefLabel or skos:altLabel) or that define them (e.g. rdfs:comment or dc:description). This pitfall is related to the guidelines provided in [5].*

    

#### P22. Using different naming conventions in the ontology <img src="https://raw.githubusercontent.com/OnToology/oops-report/master/sample/minor.png" height="15px"> (1 cases detected).
*The ontology elements are not named following the same convention (for example CamelCase or use of delimiters as &quot;-&quot; or &quot;_&quot;) . Some notions about naming conventions are provided in [2].*

    




### References:
1. Gómez-Pórez, A. Ontology Evaluation. Handbook on Ontologies. S. Staab and R. Studer Editors. Springer. International Handbooks on Information Systems. Pp: 251-274. 2004.
2. Noy, N.F., McGuinness. D. L. Ontology development 101: A guide to creating your first ontology. Technical Report SMI-2001-0880, Standford Medical Informatics. 2001.
3. Rector, A., Drummond, N., Horridge, M., Rogers, J., Knublauch, H., Stevens, R.,; Wang, H., Wroe, C. ''Owl pizzas: Practical experience of teaching owl-dl: Common errors and common patterns''. In Proc. of EKAW 2004, pp: 63-81. Springer. 2004.
4. Hogan, A., Harth, A., Passant, A., Decker, S., Polleres, A. Weaving the Pedantic Web. Linked Data on the Web Workshop LDOW2010 at WWW2010 (2010).
5. Archer, P., Goedertier, S., and Loutas, N. D7.1.3 - Study on persistent URIs, with identification of best practices and recommendations on the topic for the MSs and the EC. Deliverable. December 17, 2012.
6. Heath, T., Bizer, C.: Linked data: Evolving the Web into a global data space (1st edition). Morgan & Claypool (2011).

