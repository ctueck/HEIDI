# HEIDI
Higher Education Interoperable Data Initiative

## Problem Definition and Goal

There are a number of data-related projects and systems in European higher education, tackling student data, statistics or databases of institutions, amongst others. At the moment, we are not really interoperable. This creates costs, ineffeciencies and lack of transparency.

We would like to see these projects/systems interoperate seamlessly and thus serve best a large number of users in the European higher education community. Better linking the various data sets and systems would maximise their potential, transferring or correlating data between different systems may open entirely new use cases or valuable insights.

### Problem Domains

There are a number of problem domains, some more pressing than others. The following inventory is in order of priority:

#### Identifiers

Identifiers are needed to unambiguously identify entities when communicating or transfering data between systems. The following entities frequently need to be identified in higher education:

1. Countries and higher education systems
1. Higher education institutions
1. Study programmes
1. Courses or modules
1. Students

For countries, ISO codes are established identifiers.

Higher education institutions are a pivotal enitity, institutional identifiers thus a matter of priority. Various approaches already exist (e.g. PIC, ETER, Erasmus Code, EIDAS), but are not articulated to each other. At the same time, given less than 10000 HEIs in Europe the numbers are relatively managable.

For study programmes, courses and students numbers are larger by magnitudes.

For students, a European Student ID is under development as a federated/delegated system based on institutional student IDs.

**To add:** overview of existing course or programme identifiers, if any

#### Data Structure

Different systems should use agreed data models/structures, or at least make the data models/structures they use fully transparent. This will allow easy communication and conversion of data between systems.

At European level, it might be useful to agree on common data formats for describing:

1. Information on countries and their higher education system(s)
1. Basic information on higher education institutions
1. Information on study programmes
1. Information on quality assurance (of an institution or programme)
1. Information on student achievements (credits)
1. Information on a qualification awarded

Different organisations, dealing with such data, have already developed their data models. These should be used as a starting point.

#### Data Availability

Data on students and their achievement is personal data and will thus generally be private.

All other data discussed herein (institutions, courses, etc.) is inherently public. In addition to being accessible through a public web interface, all projects/systems should also make their data fully open and accessible for download or through an API.

#### Data Portability
#### Other Issues

## Initiatives Requiring Interoperability

There are numerous local, regional, national, European and international initiatives that deal with data in higher education. In the beginning, HEIDI aims to bring together the essential European-level projects and systems, focusing on publicly-funded or publicly-endorsed ones.

- Europass Digital Credentials Infrastructure (EDCI)
- Erasmus Without Papers (EWP)
- Emrex (implementing ELMO spec)
- European Student Card (ESC)
- My Academic ID
- Database of External Quality Assurance Results (DEQAR)
- European Tertiary Education Register (ETER)
- DiploMe?
- IAU WHED?

## Design Requirements for an Interoperability Initiative

Given the rapid progress of these initiatives and the policy priority attached to digitalisation, the Initiative needs to be able to act and reach agreement on crucial standards quickly.

### Scope

It is suggested that the Initiative focuses on higher education within the 48 countries making up the European Higher Education Area (EHEA). (Nevertheless, results might be scalable geographically or transferable to other sectors later on.)

### Governance Requirements

The Initiative should be stakeholder-led, that is, driven by the initiatives concerned. The organisations running these initiatives have expertise in their field and are best-placed to agree on standards jointly.

It should be ensured that the European Commission, governments and further stakeholders (e.g. European representative organisations) endorse the Initiative's efforts and standards. Given the scope, this could be best achieved by informing the EHEA's working structures, i.e. the Bologna Follow-Up Group (BFUG), and possibly suggesting that the Initiative become part of the 2020-2023 EHEA work programme.

The Initiative recognises that different organisations each manage specific initiatives/systems within their own remit, and does not aim to change these.

### Licence Requirements
Free (as in air)

### Use-Case (Sector-Specific) Requirements
There must be a link to QA data

### Technical Requirements

#### Linked Open Data
We propose that all interoperability should be based around the concept of [Linked Open Data](https://www.w3.org/wiki/LinkedData). Tim Berners Lee, the creator of the web has published guidelines for Linked Open Data through the W3. These encompass four rules, and a ‘quality classification’. The four rules for linked data are:

1. Use URIs as names for things
1. Use HTTP URIs so that people can look up those names.
1. When someone looks up a URI, provide useful information, using the standards (RDF, SPARQL)
1. Include links to other URIs. so that they can discover more things.

The quality conventions around Linked Open Data envisage 5 star levels of open data. The 5 Star Linked Data system is cumulative. Each additional star presumes the data meets the criteria of the previous step(s).

☆ Data is available on the Web, in whatever format.	

☆☆ Available as machine-readable structured data, (i.e., not a scanned image).

☆☆☆ Available in a non-proprietary format, (i.e, CSV, not Microsoft Excel).	

☆☆☆☆ Published using open standards from the W3C (RDF and SPARQL).	

☆☆☆☆☆ All of the above and links to other Linked Open Data.

#### Serialisaiton
RDF
JSON-LD
XML

#### Infrastructure Considerations

Responsibilities for various data and systems are distributed between institutional, national and European levels, as well as between different organisations or consortia at the European level. The Initiative seeks to achieve necessary harmonisation between different systems, while respecting their remits and autonomy. In doing so, three classes of solutions present themselves, each with varying degrees of privacy protections and distribution of control. HEIDI should in its early stages make a commitment to one of these infrastructural models, or to hybrid systems that combine elements of the models:

##### Centralised
HEIDI does not aim to centralise infrastructure or responsibilities. Instead, the aim is to mutually agree on standards to allow our  systems to interact. Each organisation should remain responsible for its infrastructure and for implementing the agreed standard(s) within the system(s) it manages. (Under such a model, communciation would occur: Institution A -->  Repository --> Institution B) Centralised databases support this model.

##### Distributed
A distributed model implies a central role for a 'clearinghouse' of institutional data, which has a central role in connecting all federated databases to each other. Under such a model the clearinghouse would link identifiers to one another, route requests and perform other similar functions. (Institution A --> Hub A -->  Clearinghouse --> Hub  B --> Institution B) Technologies such as centralised mapping/conversion tables support this use case.

##### Decentralised Gatekeepers
In a decentralised gatekeepers model, a new decentralised network made up of other networks (each of which may centralised, distribtued or decentralied in itself). Each network would be fully fully autonomous, but a set of protocols would govern how they interact with each other. Thus data exchange would happen on the folowing flow: (Institution A --> Hub A --> Hub  B --> Institution B) Technologies such as stamdardsed API Frameworks support this use model

##### Fully Decentralised
In a fully decentralised model, each institution receives a generic decentralised identifier which it uses to manage its identity. It may receive further identifiers which it collects in its wallet from other networks, but it remains the source for its identity. Under this model, all identifiers except the DID become verifiable credentials issued by other organisations. Data Exchange can happen on the followin flow (Institution A --> Institution B). A crop of emerging standards such as W3C DID and W3C support these implemenetations.



## Applications & Priorities

The following sections list concrete problem domains that should be tackled, in order of priority:

### Higher Education Institution Identifiers

Given their crucial importance, we suggest that Higher Education Institution Identifiers be the first problem domain to be concretely addressed.
The following 
[whitepaper](https://github.com/anthonycamilleri/HEIDI/blob/master/HEIDI%20HEI%20Identifiers%20Whitepaper.md) discusses options for HEI Identifiers.

### Course Identifiers

If HEI Identifiers are solved, it becomes easy to solve course identifiers, via a specification that sets a course identifier as HEI Identifier/Course Identifier. We therefore would propose addressing this issue after HEI Identifiers

Other problem domains should be added over time

## Coordinating Structure

A range of informal conversations were held on the need to address interoperability between a range of individuals and initiatives throughout 2019.

((organisations)) agreed to jointly convene a first meeting ... In its [DEQAR CONNECT project](https://www.eqar.eu/kb/projects/deqar-connect/), EQAR undertook to convene a roundtable of higher education data-related projects and initiatives.

