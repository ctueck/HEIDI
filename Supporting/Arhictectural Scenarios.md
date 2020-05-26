# Arhictectural Scenarios

## Linked Open Data
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

## Serialisaiton Options
RDF
JSON-LD
XML

## Infrastructure Considerations

Responsibilities for various data and systems are distributed between institutional, national and European levels, as well as between different organisations or consortia at the European level. The Initiative seeks to achieve necessary harmonisation between different systems, while respecting their remits and autonomy. In doing so, three classes of solutions present themselves, each with varying degrees of privacy protections and distribution of control. HEIDI should in its early stages make a commitment to one of these infrastructural models, or to hybrid systems that combine elements of the models:

### Centralised
HEIDI does not aim to centralise infrastructure or responsibilities. Instead, the aim is to mutually agree on standards to allow our  systems to interact. Each organisation should remain responsible for its infrastructure and for implementing the agreed standard(s) within the system(s) it manages. (Under such a model, communciation would occur: Institution A -->  Repository --> Institution B) Centralised databases support this model.

### Distributed
A distributed model implies a central role for a 'clearinghouse' of institutional data, which has a central role in connecting all federated databases to each other. Under such a model the clearinghouse would link identifiers to one another, route requests and perform other similar functions. (Institution A --> Hub A -->  Clearinghouse --> Hub  B --> Institution B) Technologies such as centralised mapping/conversion tables support this use case.

### Decentralised Gatekeepers
In a decentralised gatekeepers model, a new decentralised network made up of other networks (each of which may centralised, distribtued or decentralied in itself). Each network would be fully fully autonomous, but a set of protocols would govern how they interact with each other. Thus data exchange would happen on the folowing flow: (Institution A --> Hub A --> Hub  B --> Institution B) Technologies such as stamdardsed API Frameworks support this use model

### Fully Decentralised
In a fully decentralised model, each institution receives a generic decentralised identifier which it uses to manage its identity. It may receive further identifiers which it collects in its wallet from other networks, but it remains the source for its identity. Under this model, all identifiers except the DID become verifiable credentials issued by other organisations. Data Exchange can happen on the followin flow (Institution A --> Institution B). A crop of emerging standards such as W3C DID and W3C support these implemenetations.