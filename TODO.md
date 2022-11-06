- have a spinner while waiting
- filter away all successes in the results on the bottom
- allow to start from a specific prefix
- what happens if you move back into a previous field
- make input choice selectable
- conditions (grammatical gender, etc)

For conditions:
select distinct ?p {
  ?lexemeId a ontolex:LexicalEntry .
  ?lexemeId dct:language wd:Q6654 .
  ?lexemeId wikibase:lexicalCategory wd:Q1084 .
  ?lexemeId ?p ?o .
  ?p a owl:ObjectProperty .
  ?s wikibase:directClaim ?p .
}