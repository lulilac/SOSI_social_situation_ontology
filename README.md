# SOSI – Social Situation Ontology

SOSI (Social Situation Ontology) is an OWL ontology designed to represent and categorize **social situations in Human–Robot Interaction (HRI)**.
The ontology provides a structured representation of interaction contexts, participants, communicative behaviors, and situational dynamics occurring during social interactions involving humans and robots.

SOSI enables researchers to **formally describe, annotate, and analyze social situations**, facilitating reproducibility and interoperability across HRI studies and datasets.

The conceptual structure of the ontology is inspired by **Kenneth Burke’s Dramatistic Pentad**, a framework traditionally used to analyze human actions through five elements: **Act, Scene, Agent, Agency, and Purpose**.

---

# Conceptual Foundation

SOSI is grounded in the analytical framework proposed by Kenneth Burke known as the **Dramatistic Pentad**.
This framework describes human action through five core components:

* **Act** – what is happening
* **Scene** – the context in which the action occurs
* **Agent** – the actors involved in the action
* **Agency** – the means or modalities through which the action is performed
* **Purpose** – the intention or goal behind the action

SOSI adapts this framework to structure and categorize **observable elements of social situations**, particularly those relevant to **human–robot interaction research**.

Rather than modeling narrative discourse, the ontology focuses on **empirical interaction characteristics** that can be observed, annotated, and analyzed during social interaction scenarios.

---

# Ontology Overview

The core concept of SOSI is the class:

**SocialSituation**

A `SocialSituation` represents an interaction context involving one or more agents and is characterized through multiple descriptive dimensions derived from Burke’s Pentad.

These dimensions describe:

* the **environment** in which the interaction occurs
* the **participants** involved
* the **type of interaction** taking place
* the **communication modalities** used
* the **goal or purpose** of the interaction

Together, these dimensions provide a structured representation of complex social interactions.

---

# Core Ontology Dimensions

## Scene – Interaction Context

The **Scene** dimension represents the situational and environmental context in which the interaction occurs.

It describes the physical and social environment surrounding the interaction.

Typical contextual properties include:

* location of the interaction
* type of physical environment (e.g., indoor or outdoor)
* level of formality
* social background context

Example properties used in the ontology:

* `hasLocation`
* `hasPhysicalType`
* `hasFormality`
* `hasCrowdContextBg`

These attributes characterize the situational setting that influences social behavior.

---

## Agent – Participants

The **Agent** dimension represents the actors involved in the interaction.

In HRI scenarios, agents may include:

* humans
* robots
* groups of participants

This dimension describes both the **number of participants** and the **social relationships** between them.

Relevant properties include:

* `hasCardinality` – number of participants
* `hasRelationType` – type of relationship between participants (e.g., strangers, acquaintances, colleagues)

These attributes allow the ontology to represent the **social structure of the interaction**.

---

## Act – Interaction Type

The **Act** dimension represents the **type of social interaction occurring between agents**.

It describes the nature of the activity or interaction dynamics.

Examples of interaction types include:

* cooperative interactions
* competitive interactions
* persuasive interactions
* observational interactions
* conforming interactions

The ontology models this dimension primarily through:

* `hasInteractionType`

Additional interaction dynamics are also represented through:

* engagement level
* interdependence level between participants

These attributes characterize the **behavioral structure of the interaction**.

---

## Agency – Communication Modalities

The **Agency** dimension represents **how the interaction is performed**, focusing on communication behaviors and modalities.

In social interactions, agents communicate through both **verbal** and **nonverbal signals**.

SOSI captures these communication mechanisms through properties such as:

* `hasSpeechActivity`
* `hasNonverbalSignaling`
* `hasNonverbalCue`
* `hasProxemicsValue`
* `hasRelativeBodyPlacement`

These properties allow the ontology to represent aspects such as:

* presence of speech
* eye contact
* body orientation
* spatial distance between participants
* gesture or other nonverbal signals

These communication cues are central to modeling **social behavior in human–robot interaction**.

---

## Purpose – Interaction Goal

The **Purpose** dimension represents the **goal or intention behind the interaction**.

This is modeled through the property:

* `hasPurpose`

The purpose describes the objective that motivates the interaction.

Examples include:

* completing a collaborative task
* providing assistance
* greeting someone
* exchanging information
* guiding a user

The purpose dimension provides a semantic representation of **why the interaction occurs**.

---

# Additional Interaction Dimensions

Beyond the five pentadic components, SOSI also models **affective and engagement-related characteristics** of social interactions.

These dimensions capture aspects of interaction quality and participant involvement.

## Emotional Valence

The emotional tone of the interaction is represented through:

`hasEmotionalValence`

Possible values may include:

* positive
* neutral
* negative

This dimension describes the **emotional atmosphere of the interaction**.

---

## Engagement Level

The degree to which participants are actively involved in the interaction is represented through:

`hasEngagementLevel`

Example levels include:

* engaged
* disengaged
* mixed

This allows the ontology to represent **participation intensity** during the interaction.

---

## Interdependence Level

The level of dependency between participants during the interaction is represented through:

`hasInterdependenceLevel`.

This dimension captures whether participants must strongly rely on each other to complete the interaction.

Examples include:

* low interdependence
* moderate interdependence
* high interdependence

---

# Example Representation

An example social situation described using SOSI could be:

* **Location:** indoor office environment
* **Participants:** small group
* **Relation type:** colleagues
* **Interaction type:** cooperative task
* **Speech activity:** present
* **Nonverbal cues:** eye contact and body orientation
* **Engagement level:** engaged
* **Emotional valence:** positive

This structured description enables consistent annotation of social interaction scenarios.

---

# Applications

SOSI can support several research and technical applications, including:

* annotation of **human–robot interaction experiments**
* creation of **social interaction datasets**
* representation of **interaction scenarios for social robots**
* analysis of **behavioral dynamics in social contexts**
* knowledge representation for **socially intelligent robotic systems**

---

# Implementation

The ontology is implemented using:

* **OWL (Web Ontology Language)**
* **RDF**
* **Turtle (.ttl) serialization**

Namespace:

http://www.phd-project.org/ontology/sosi#

---

# Repository Structure

```
sosi.ttl
    Main ontology file containing the SOSI ontology in Turtle format

README.md
    Documentation describing the ontology and its conceptual framework
```

---

# Potential Use in Human–Robot Interaction Research

The ontology is particularly suited for:

* structuring experimental scenarios in HRI studies
* describing contextual variables in interaction experiments
* annotating behavioral datasets
* supporting reasoning about social interaction contexts in robots

By grounding interaction representation in a formal ontology, SOSI promotes **consistent modeling of social situations across different studies and systems**.

---

# License

Specify the license under which the ontology is distributed (e.g., MIT License, Creative Commons, etc.).

---

# Author

Developed as part of research on **social situation modeling for Human–Robot Interaction (HRI)**.
