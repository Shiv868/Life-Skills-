# Full Text Search Performance Investigation

## Introduction

Full Text Search is a technique used to search large volumes of unstructured text data efficiently. It supports keyword matching, phrase search, filtering, and relevance ranking. In our new project, the current database driven search system is facing performance and scaling problems due to increasing data size and user traffic. Traditional relational database queries are not optimized for advanced text searching. Hence, the team lead assigned an investigation to evaluate specialized Full Text Search technologies.

## Problem Statement

The existing system uses SQL LIKE queries and basic indexing, which causes several issues:

* Slow query response time  
* Limited search relevance ranking  
* High database load  
* Poor scalability with data growth  

To resolve these challenges, three technologies were analyzed.

## Technologies Evaluated

### Elasticsearch

* Distributed and horizontally scalable  
* Near real time indexing  
* REST API for easy integration  
* Built in analytics and aggregation  

### Apache Solr

* Enterprise grade search platform  
* Advanced caching mechanisms  
* Faceted search support  
* Highly configurable schema design  

### Apache Lucene

* High performance search library  
* Low level indexing control  
* Lightweight and embeddable  
* Requires custom implementation  

## Comparative Analysis

1. Scalability: Elasticsearch and Solr support distributed scaling.  
2. Integration: Elasticsearch is easier using REST APIs.  
3. Customization: Lucene offers maximum flexibility.  
4. Performance: Elasticsearch performs best for real time large datasets.  

## Conclusion

Implementing a dedicated Full Text Search engine will improve search speed and system scalability. Elasticsearch is the most suitable solution due to its distributed architecture and ease of deployment. Solr fits enterprise customization needs, while Lucene is ideal for embedded search applications.

## References

* https://www.elastic.co/guide/index.html  
* https://solr.apache.org/guide/  
* https://lucene.apache.org/core/documentation.html  
* https://www.elastic.co/what-is/elasticsearch  
* https://en.wikipedia.org/wiki/Full-text_search
