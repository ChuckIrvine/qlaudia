# From Field to Knowledge: A Minimal Ontology for Generative AI Tutoring Systems

## Chapter 1. Introduction

### Motivation
Generative AI has shown remarkable ability to create text, images, and code. Yet its outputs, while fluent, are often ungrounded: they lack a structured foundation for knowledge. Human language is expressive but also ambiguous and culturally relative. Knowledge graphs and ontologies, on the other hand, often collapse under their own weight—too many categories, inconsistent hierarchies, and brittle structures.

Education is a clear domain where these weaknesses show. AI tutors can answer questions conversationally, but they lack a systematic, minimal foundation for teaching. Without such a foundation, explanations are shallow, student progress is hard to measure, and true adaptive learning remains elusive.

### Core Idea
This dissertation proposes a framework for codifying knowledge based on a **two-layer ontology**:  

- **Layer 0 (Ontological Ground): Field**  
  - The continuous, undifferentiated reality from which all else emerges.  
  - Cannot itself be directly codified, only approximated through projections.  

- **Layer 1 (Emergent Primitives):**  
  1. **Substance** — coherence or presence that arises from the field.  
  2. **Relation** — structured connectedness between substances.  
  3. **Change** — transformation of substances or relations.  
  4. **Extent** — spread or dimensionality of substances and changes.  

From these primitives, **derivative concepts** emerge: Objects, Magnitudes, Events, Laws, Systems, and higher constructs. This codification enables generative AI to move beyond free-form text, supporting a **Virtual Teacher** that guides learners by traversing structured knowledge.

### Research Questions
1. Can all subject matter be codified using the four emergent primitives (Substance, Relation, Change, Extent)?  
2. How efficient, accurate, and minimal is this codification compared to existing ontological approaches?  
3. Can a codified knowledge base serve as the substrate for a generative Virtual Teacher?  

### Contributions
- A redefined ontology: Field (ground) → Primitives (SRC-E) → Derived Taxonomy.  
- A codification pipeline from natural language to structured primitives.  
- A prototype implementation codifying educational material.  
- Evaluation in terms of fidelity, compression, and educational usefulness.  

---

## Chapter 2. Literature Review

### Philosophical Roots

- **Heraclitus (c. 500 BCE)**: Known for the doctrine of *flux*, Heraclitus argued that reality is in constant motion. Stability is an illusion. This resonates with **Change** as a primitive, and with objects understood as temporary configurations of substance.  

- **Spinoza (1632–1677)**: In *Ethics*, Spinoza asserted that all things are modes of a single **Substance**. Finite things do not exist independently but emerge from the infinite. This aligns with our distinction: **Substance emerges from the Field**, while objects are bounded forms of substance.  

- **Whitehead (1861–1947)**: Developed *Process and Reality*, emphasizing that the fundamental units of reality are events rather than substances. His “actual occasions” echo our primitive of **Change** and highlight the processual nature of being.  

- **David Bohm (1917–1992)**: Proposed the *Implicate Order*, a holistic **Field** from which the explicate order of objects emerges. This directly supports our framework: Field (Layer 0) giving rise to Substance and further primitives (Layer 1).  

- **Anna Wierzbicka (1941–)**: In developing the *Natural Semantic Metalanguage*, Wierzbicka identified universal semantic primes. Her work demonstrates the feasibility of building meaning systems from minimal, irreducible primitives—paralleling our attempt with Substance, Relation, Change, and Extent.  

### Knowledge Representation in AI

- **Semantic Networks (1960s–1970s)**: Quillian’s semantic memory and Minsky’s frames represented knowledge as graphs of nodes and relations. These early systems foreshadowed the importance of **Relation** as a primitive.  

- **Expert Systems (1970s–1980s)**: Rule-based systems like MYCIN encoded knowledge symbolically but were brittle and difficult to extend. Their struggles underscored the need for **minimal, general primitives** rather than sprawling rules.  

- **Knowledge Graphs**:  
  - **WordNet (1985)**: organized words into synonym sets, mapping lexical relations but tied to English.  
  - **Cyc (1984–)**: attempted to encode all common sense in a vast ontology. Its overgrowth showed the pitfalls of excessive categories.  
  - **ConceptNet (1999–)**: crowdsourced relational knowledge, but noisy and imprecise.  
  - **Wikidata (2012–)**: large-scale, structured, multilingual, but inherits redundancy and category sprawl from natural language.  

- **Ontology Engineering (1990s–)**: RDF, OWL, and related standards introduced rigor and formalism but required expert curation and were often domain-specific. They do not offer a universal, minimal foundation.  

**Conclusion:** Both philosophy and AI research suggest that knowledge requires grounding in primitives. What has been missing is a universal, minimal, field-emergent set of primitives—precisely what this dissertation proposes.  

---

## Chapter 3. Theoretical Framework

### Two-Layer Ontology
- **Layer 0: Field**  
  The ontological ground: continuous, undifferentiated, and beyond direct codification. The Field is real but cannot be captured directly. It is the generative ground.  

- **Layer 1: Emergent Primitives**  
  From the Field arise four codifiable primitives:  
  1. **Substance**: coherent presences emerging from the field.  
  2. **Relation**: structured connections between substances.  
  3. **Change**: transformations of substances or relations over time.  
  4. **Extent**: spread, scope, or dimensionality inherent in substances and changes.  

### Derived Concepts
- **Object**: bounded configuration of substance.  
- **Magnitude**: relative measure of extent, defined through comparison or convention.  
- **Event**: a change involving one or more substances and relations across extent.  
- **Law**: relation linking changes and extents into regular patterns.  
- **System**: a network of objects, relations, changes, and extents functioning as a whole.  

### Composite Examples
- **Truth**: a relation between perception and substance/change that preserves fidelity.  
- **Time**: a structured description of change expressed through extent.  
- **Causation**: a relation between changes, quantified by extents and expressed via magnitudes.  

### Hypothesis
All subject matter—scientific, mathematical, social, artistic—can be expressed through this structure. New categories may be added only when primitives and derivatives fail, preserving minimalism.  

---

## Chapter 4. Methodology: Codification Pipeline

### Input
Textual material from any subject domain (e.g., textbooks, scientific articles, transcripts).  

### Processing Stages
1. **Segmentation**: Break source text into atomic claims.  
2. **Extraction**: Use generative AI constrained by schema to express claims in terms of primitives (Substance, Relation, Change, Extent).  
3. **Normalization**: Resolve duplicates, unify terminology, standardize extents (units, dimensions).  
4. **Composition**: Build higher-level constructs (objects, magnitudes, events, laws, systems) from recurring primitives.  
5. **Validation**: Perform internal checks (unit consistency, logical coherence) and external checks (round-trip fidelity from codified form back to natural language).  

### Output
A codified knowledge graph structured by primitives and derivatives, linked to original sources for provenance.  

### Evaluation Metrics
- **Coverage**: proportion of content successfully codified.  
- **Compression**: reduction relative to raw text.  
- **Fidelity**: degree to which regenerated explanations match original text.  
- **Minimality**: stability of taxonomy and avoidance of uncontrolled category growth.  

### Taxonomy Governance
New derivative categories may be proposed when primitives fail, but only adopted with rigorous justification. This ensures that the taxonomy grows slowly and deliberately, preserving its universality and minimalism.  

---
