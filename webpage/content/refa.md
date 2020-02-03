+++
date = "2019-02-12"
title = "Refactoring Tutorials@iFM"
type = "general" 
+++

# **Refactoring Tutorials-iFM'19**\

Supported by the bilateral Norwegian-Brazilian project ["Modern Refactoring"](https://ict.hvl.no/modern-refactoring/) (DIKU/CAPES, 2017-2020).

### Date: Monday, 2 December 2019

### Program ####

* ***9:00-10:00 [Introduction & Overview](#intro)***  
 [Volker Stolz](http://ict.hvl.no/people/volker-stolz/) (Høgskulen på Vestlandet)
* ***10:00-10:30 Coffee break***
*  ***10:30-12:00 [Model refactoring with relational Reference Attribute Grammars](#rag)***  
[Johannes Mey, René Schöne, Uwe Aßmann](https://tu-dresden.de/ing/informatik/smt/)
(TU Dresden, Germany),  
Niklas Fors, [Görel Hedin](http://cs.lth.se/gorel-hedin/) (University of Lund, Denmark)
* ***12:00-12:30 [Revisiting the refactoring mechanics](#rohit)***  
[Rohit Gheyi](http://www.dsc.ufcg.edu.br/~rohit/) (Universidade Federal de Campina Grande, Brazil)
* ***12:30-14:00 Lunch***
* ***14:00-14:45 [Studying the Relationship between refactoring and code review](#tiago)***  
[Tiago Massoni](https://massoni.computacao.ufcg.edu.br) (Universidade Federal de Campina Grande, Brazil)
* ***14:45-15:30 [How to Prove the Correctness of Refactoring Rules](#pcrr)***  
 [Dominic Steinhöfel, Reiner Hähnle](https://www.informatik.tu-darmstadt.de/se/homepage/) (TU Darmstadt, Germany)
* ***15:30-16:00 Coffee break***
* ***16:00-16:45 "How to Prove..."*** continued
* ***16:45 Short presentations by participants***

---

## Abstracts

### <a id="intro">Introduction and Overview</a>
[Volker Stolz](http://ict.hvl.no/people/volker-stolz/) (Høgskulen på Vestlandet):

<div style="text-align: justify;">
Refactoring is an important software engineering task. In this tutorial, we will first look at the underlying principles and the improvements we can expect from refactoring code. Then, we compare refactoring support in common integrated development environments (IDEs) and editors for popular programming languages. We will also discuss the limitations of current tools, and give potential research directions (ranging in difficulty from a Master thesis project to problems that are very well worth a PhD).
</div>

---

### <a id="rag">Model refactoring with relational Reference Attribute Grammars</a>

[Johannes Mey, René Schöne, Uwe Aßmann](https://tu-dresden.de/ing/informatik/smt/)
(TU Dresden, Germany),  
Niklas Fors, [Görel Hedin](http://cs.lth.se/gorel-hedin/) (University
of Lund, Denmark):

<div style="text-align: justify;">
Reference Attribute Grammars annotate nodes in syntax trees of context-free grammars with attributes, which specify computed properties of those nodes and may also take the form of references to other nodes in the same tree (reference attributes).
This approach can also be used for the analysis of conceptual models by using reference attributes to specify cross-tree relations.
Furthermore, RAGs support extended features to modify a tree, such as simple tree edits, higher-order attributes, and incremental evaluation after an edit.
Relational RAGs is a further extension of the concept that introduces intrinsic bidirectional cross-tree relations, which has been shown to allow an efficient re-evaluation of attributes while maintaining consistency after modification.
In this workshop, we will introduce (relational) RAGs, demonstrate how a conceptual model can be transformed into a grammar and relation definition, and illustrate how attributes can be used to efficiently yet consistently refactor a model.
This workshop will work on Ecore models using the RAG system JastAdd with a relational RAG extension.
</div>

---

### <a id="pcrr">How to Prove the Correctness of Refactoring Rules</a>

[Dominic Steinhöfel, Reiner Hähnle](https://www.informatik.tu-darmstadt.de/se/homepage/) (TU Darmstadt, Germany):  

<div style="text-align: justify;">
We present a new static software analysis principle called
   Abstract Execution (AE) which allows to symbolically execute a
   partially unspecified (schematic) program with placeholder
   symbols. For each such abstract symbol, we faithfully represent
   all possible concrete executions resulting from its substitution
   with concrete code. There is a wide range of applications of AE,
   especially for verifying relational properties of schematic
   programs. We implemented AE in the verification framework KeY and
   proved correctness of eight well-known statement-level refactoring
   rules, including two with loops. For each refactoring we
   characterize the preconditions that make it semantics-preserving.
   Most preconditions are not mentioned in the literature. In other
   words: Most refactoring rules are unsound in general, but can be
   fixed by adding further constraints.
</div>

---

### <a id="rohit">Revisiting the refactoring mechanics</a>

[Rohit Gheyi](http://www.dsc.ufcg.edu.br/~rohit/) (Universidade Federal de Campina Grande, Brazil)

<div style="text-align: justify;">
Refactoring is a key practice in agile methodologies used by a number of developers, and available in popular IDEs. However, it is unclear whether the refactoring mechanics have the same meaning for developers.
In this talk, we revisit the refactoring mechanics.
We conduct a survey with 107 developers of popular Java projects on GitHub. We asked them about the output of seven refactoring types applied to small programs.
Developers do not expect the same outputs in all questions. The refactoring mechanics is based on developers’ experience for a number of them (71.02%). Some developers (75.70%) use IDEs to apply refactorings. However, the output yielded by the preferred IDE is different from what they want.
Developers and IDE developers use different mechanics for most refactoring types considered in our survey, and this may impact developers’ communication.
</div>

---

### <a id="tiago">Studying the Relationship between refactoring and code review</a>

[Tiago Massoni](https://massoni.computacao.ufcg.edu.br) (Universidade Federal de Campina Grande, Brazil)

<div style="text-align: justify;">
Modern Code Review (MCR) demands enhancements in the way changelogs are presented to reviewers. Their task benefits from higher-level descriptions about the intention behind commits; for instance, evolution tasks, such as refactorings, could be more effectively reviewed in the presence of the intended transformation -- better if automatically detected by MCR tool support. Furthermore, compelling research questions consider how the review process could induce refactorings and other types of evolution. Since 2015, interest in tools and techniques for automatic detection of refactorings has been steadily growing. Most publications document development methods or carry out characterization studies. We point out a few potential research topics for the next years. In particular, detection of multiple refactoring types in a mixed changelog (in which refactorings are combined with other kinds of changes), or the need for case studies or experiments in applying refactoring detection in MCR, on distinct application domains and development environments.
</div>
