# Regulation Innovation SIG Demo Summaries

Below is a list of the solutions and use cases that have been presented at [Regulation Innovation SIG meetings](https://github.com/finos/open-regtech-sig/issues?q=label%3Ameeting). 

If you presented at a Regulation Innovation SIG meeting and your demo is not included below, feel free to submit a PR to add it, and reach out to help@finos.org if you need assistance.

## Morphir
Presented by Morgan Stanley at the [November 24th 2020 Regulation Innovation SIG meeting](https://github.com/finos/open-regtech-sig/issues/10)

### Overview
Morphir is a multi-language system built on a data format that captures an application’s domain model and business logic in a technology agnostic manner. Having all the business knowledge available as data allows you to process it programatically in various ways:
- Translate it to move between languages and platforms effortlessly as technology evolves
- Visualize it to turn black-box logic into insightful explanations for your business users
- Share it across different departments or organizations for consistent interpretation
- Store it to retrieve and explain earlier versions of the logic in seconds
- and much more …
Learn more at [morphir.finos.org](https://morphir.finos.org) and check out the open source code at [github.com/finos/morphir](https://github.com/finos/morphir).

### Opportunity for Open Source Collaboration
There are quite a few open-source and proprietary solutions that address the ontology (including rules and calculations) portion of this initiative. At their cores, they all function very similarly, though because they’ve evolved independently are not directly compatible. Most have advanced and mature features that we’d want to take advantage of. So rather than choosing one, we should aim to provide a standardized mechanism for interoperability that would allow us to take advantage of the full set of existing features while also enabling new tool developers to work efficiently on a common platform. 
 
That’s where Morphir fits in; as that common structure (IR) that we can use to translate between the various solutions and focus new development on. There’s no shortage of options to try this on and ISDA and Regnosys being forward thinking and similarly aligned stepped up with a use case. 
 
The first goal is to see how CDM/Rosetta concepts translate to Morphir. We’re looking at that by first writing a subset of CDM in Morphir by hand to serve as a template. With that established, we’ll look into automating the rest. We might want to look at translating Morphir back to Rosetta and use that round trip as a template for using Morphir as the lingua franca between the various solutions.
 
Another goal is to see how we would write the same regulations in more idiomatic Morphir in order to take advantage of the correctness guarantees, etc. That would allow us to study and compare the two approaches for managing complex regulations, especially with respect to correctness, transparency, and flexibility.

## Rosetta CDM
Presented by Regnosys at the [November 24th 2020 Regulation Innovation SIG meeting](https://github.com/finos/open-regtech-sig/issues/10)

### Overview
Rosetta Core is a complete Software Development Kit (SDK or dev kit) for the Rosetta DSL. It consists of an integrated set of tools for adopting, editing and implementing any model built on the Rosetta DSL. The ISDA Common Domain Model (CDM) is the first live application of the Rosetta DSL and is currently provided as the underlying model in Rosetta Core.

This means that users of Rosetta Core do not need to start modelling “from scratch” and can leverage the existing ISDA CDM components. This also means that Rosetta Core provides an integrated set of tools for adopting, editing and implementing the ISDA CDM.

### Opportunity for Open Source Collaboration
One of the applications of the Rosetta DSL is to facilitate the process of complying with, and supervising, financial regulation – in particular, the large body of data reporting obligations that industry participants are subject to.

The current industry processes to implement those rules are costly and inefficient. They involve translating pages of legal language, in which the rules are originally written, into business requirements which firms then have to code into their systems to support the regulatory data collection. This leads to a duplication of effort across a large number of industry participants and to inconsistencies in how each individual firm applies the rules, in turn generating data of poor quality and comparability for regulators.

By contrast, a domain-model for the business process or activity being regulated provides standardised, unambiguous definitions for business data at the source. In turn, these business data can be used as the basis for the reporting process, such that regulatory data become unambiguous views of the business data. The Rosetta DSL allows to express those reporting rules as functional components in the same language as the model of the business domain itself. Using code generators, those functional rules are then distributed as executable code, for all industry participants to use consistently in their compliance systems.

ISDA and REGnosys successfully collaborated in 2020 to demonstrate the applicability of these tools as part of [G20 Techsprint](https://www.bis.org/hub/g20_techsprint.htm). The winning solution in the Regulatory Reporting category demonstrating how the tooling could solve Derivatives reporting challenges through implementation of the MAS reporting rules.

## RegExplorer
Presented by Deloitte at the [November 24th 2020 Regulation Innovation SIG meeting](https://github.com/finos/open-regtech-sig/issues/10)

## Orchestrate 
Presented by ING at the [December 8th 2020 Regulation Innovation SIG meeting](https://github.com/finos/open-regtech-sig/issues/13)

## RegTech Taxonomy  
Presented by Apiax at the [December 8th 2020 Regulation Innovation SIG meeting](https://github.com/finos/open-regtech-sig/issues/13)

### Overview
Apiax uses an internally developed RegTech taxonomy to create the vocabulary for regulatory rule execution. One main requirement for our solution was to support diverse vocabularies and rule interpretations of our partners and clients. Our approach is inspired by ideas in Semantic Web research and existing ontologies (FIBO and its OWL-based implementation), our goal is to create a taxonomy that is expressive and flexible enough to support our use cases, while being simple enough to not require a team of ontology experts for maintenance. We are currently looking into NLP methods how to semi-automatically populate our taxonomy and support the creation of rules from legal documents.

### Opportunity for Open Source Collaboration
We see that open source and open data is an opportunity to increase interoperability of our and other RegTech solutions. We agree, as discussed in the group, that a common RegTech vocabulary (e.g. published as an open ontology) would simplify the integration with our clients and partners. We would propose to start with an analysis of a selection of regulations, implement a vocabulary/ontology for those and develop a proof of concept how such an ontology might be linked to proprietary solutions or other open ontologies like FIBO/FIRO, and how this helps in terms of interoperability.

In addition we think that an open RegTech text corpus and open RegTech language models would help to standardize further (semi-)automated text extraction approaches to populate ontologies or extract logic from regulatory documents.

## Crypto Tech Sprint
Presented by AIR at the [January 19th 2021 Regulation Innovation SIG meeting](https://github.com/finos/open-regtech-sig/issues/16)

### Overview
Cryptocurrency has become a dominant payment method for CSAM, and in the past five years there has been proliferation in the creation of cryptocurrency paywalls to gain access to the material. Unlike cash, crypto is traceable, but traditional anti-money laundering technology and current law enforcement techniques are often ineffective in detecting and intercepting it. AIR held a virtual TechSprint in October 2020 to surface new models of traceability and explore technological solutions to combat and apprehend perpetrators of these heinous crimes.

### Opportunity for Open Source Collaboration
The TechSprint brought together technologists and subject matter experts from regulatory agencies, fintechs and crypto firms, banks, consultancies and academia. Participants collaborated on a FINOS hosted GitHub repo to build solutions aimed at curtailing CSAM by detecting users through their cryptocurrency payment activities, without compromising the privacy and data security of innocent people. All the teams were invited to present their solutions to the senior leadership team at FinCEN.  

## Federated AML Knowledge Base
Presented by Tookitaki at the [January 19th 2021 Regulation Innovation SIG meeting](https://github.com/finos/open-regtech-sig/issues/16)

## AML
Presented by Matt van Buskirk (Hummingbird Regtech) at the [January 19th 2021 Regulation Innovation SIG meeting](https://github.com/finos/open-regtech-sig/issues/16)


