# Summary

The Slovak UD treebank is based on data originally annotated as part of the
Slovak National Corpus, following the annotation style of the Prague
Dependency Treebank.


# Introduction

Slovak Dependency Treebank (Slovenský závislostný korpus) was created as part
of the Slovak National Corpus at the Ľ. Štúr Institute of the Slovak Academy of
Sciences. The original annotation follows the guidelines of the Prague
Dependency Treebank (Czech), slightly modified in the spirit of Slovak
grammatical tradition. Morphological tags, lemmas and dependency relations have
been assigned manually to every word.

The present dataset is a subset of the original treebank. We automatically
selected the sentences where the two human annotators 100% agreed on the
analysis. This increases the quality and trustworthiness of the data but it
also results in selecting short sentences most of the time. An extended version
may be published in the future when manually merged and checked annotation is
available.

This subset annotated in the original PDT-like style is available separately,
see [http://hdl.handle.net/11234/1-1822](http://hdl.handle.net/11234/1-1822)
and cite as

Gajdošová, Katarína; Šimková, Mária et al., 2016,
  Slovak Dependency Treebank,
  LINDAT/CLARIN digital library at the Institute of Formal and Applied
  Linguistics, Charles University in Prague,
  http://hdl.handle.net/11234/1-1822.

UD_Slovak contains the same data with annotation converted to conform to the
Universal Dependencies guidelines. The original treebank was prepared by a team
led by Katarína Gajdošová and Mária Šimková. Selection of sentences for this
subset and conversion to Universal Dependencies was done by Dan Zeman.

## References

* Daniel Zeman (2017):
  Slovak Dependency Treebank in Universal Dependencies.
  In: Jazykovedný časopis / Journal of Linguistics, ISSN 0021-5597,
  vol. 68, no. 2, pp. 385-395


# Changelog:

* 2025-05-15 v2.16
  * Adjectives heading clauses are acl(:relcl) rather than amod.
  * Non-agreeing postponed determiners are now mostly nmod.
  * No longer distinguishing flat:foreign from flat.
  * Fixed multiword expressions need the ExtPos feature.
* 2024-05-15 v2.14
  * Added the enhanced relation subtype nsubj:xsubj.
  * More restrictive use of orphans and empty nodes: Not in non-verbal coordinated sentences.
  * Improved form and position of abstract predicates in gapping.
* 2021-05-15 v2.8
  * Fixed recognition of clauses with passive participles (ADJ).
  * Split multi-word tokens of the type "naňho".
* 2020-05-15 v2.6
  * Changed sentence ids to preserve the name of the source text.
    * Side effect: The order of the sentences changed, and so did the train-dev-test data split.
  * Genitive, dative and instrumental nominals are now considered oblique.
  * Added enhanced relations with case information.
  * Added enhanced relations around relative clauses.
  * Added enhanced external subjects in control verb constructions.
  * Added empty nodes to enhanced graphs (but orphans are just converted to dep).
* 2019-05-15 v2.4
  * Fixed some bugs identified by the new validator.
* 2018-04-15 v2.2
  * Repository renamed from UD_Slovak to UD_Slovak-SNK.
  * Added enhanced representation of dependencies propagated across coordination.
    The distinction of shared and private dependents is derived deterministically from the original Prague annotation.
* 2017-11-15 v2.1
  * Prepositional objects are now “obl:arg” instead of “obj”.
  * Instrumental phrases for demoted agents in passives are now “obl:agent”.
* 2017-03-01 v2.0
  * Converted to UD v2 guidelines.
  * Improved advmod vs. obl distinction.
  * Verb negation no longer treated as derivational morphology.
  * Distinguished numeral types.
  * Distinguished pronouns, determiners and pronominal adverbs.
  * Distinguished coordinating and subordinating conjunctions.
  * L-participles are verbs, other participles are adjectives.


=== Machine-readable metadata (DO NOT REMOVE!) ================================
Data available since: UD v1.4
License: CC BY-SA 4.0
Includes text: yes
Genre: fiction nonfiction news
Lemmas: converted from manual
UPOS: converted from manual
XPOS: manual native
Features: converted from manual
Relations: converted from manual
Contributors: Gajdošová, Katarína; Šimková, Mária; Zeman, Daniel
Contributing: elsewhere
Contact: zeman@ufal.mff.cuni.cz
===============================================================================
