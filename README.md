# Histograph

Historical geocoder, built with [Neo4j](http://neo4j.com/) and [Elasticsearch](https://www.elastic.co/products/elasticsearch). See [histograph.io](http://histograph.io/) or the GitHub repositories of one of the components for more information.

## Core components

| Name           | GitHub                                                                | Description
|:---------------|:----------------------------------------------------------------------|:-------------------------------------------------------------
| Core           | [histograph/core](https://github.com/histograph/core)                 | Consumes Redis queue and syncs Neo4j and Elasticsearch
| API            | [histograph/api](https://github.com/histograph/api)                   | Search API
| IO             | [histograph/api](https://github.com/histograph/io)                    | Input/output API
| Schemas        | [histograph/schemas](https://github.com/histograph/schemas)           | Ontology and [JSON schemas](http://json-schema.org/)
| Config         | [histograph/config](https://github.com/histograph/config)             | Configuration files
| Neo4j plugin   | [histograph/neo4j-plugin](https://github.com/histograph/neo4j-plugin) | Server plugin for Neo4j for certain graph queries
| Viewer         | [histograph/viewer](https://github.com/histograph/viewer)             | Map viewer, [React](http://facebook.github.io/react/) + [Leaflet](http://leafletjs.com/) + [D3.js](http://d3js.org/)
| Data           | [histograph/data](https://github.com/histograph/data)                 | Scripts to download and generate Histograph datasets from selection of sources (GeoNames, TGN, ...)
| Import         | [histograph/import](https://github.com/histograph/import)             | Scripts to import data into Histograph API
| Stats          | [histograph/api](https://github.com/histograph/stats)                 | Runs set of queries on a specified interval to compute data statistics
| Website        | [histograph/api](https://github.com/histograph/histograph.github.io)  | Histograph website on [histograph.io](http://histograph.io)
| Fuzzy dates    | [histograph/api](https://github.com/histograph/fuzzy-dates)           | Parses dates, years, and ranges
| URI normalizer | [histograph/api](https://github.com/histograph/uri-normalizer)        | Converts URIs and Histograph IDs to URNs
| Tests          | [histograph/api](https://github.com/histograph/tests)                 | Test suite for Histograph API

## Graphmalizer

Histograph uses Graphmalizer to convert the stream of messages from the message queue (create/delete/update of PITs and relations) to a graph in Neo4j.

| Name              | GitHub                                                                              | Description
|:------------------|:------------------------------------------------------------------------------------|:-------------------------------------------------------------
| Graphmalizer Core | [graphmalizer/graphmalizer-core](https://github.com/graphmalizer/graphmalizer-core) | Reads message queue, creates Neo4j graph

## Tools

| Name            | GitHub                                                                      | Description
|:----------------|:----------------------------------------------------------------------------|:--------------------------------------------------------------------
| AWS tools       | [histograph/aws](https://github.com/histograph/aws)                         | Tools and scripts for deploying Histograph on Amazon Web Services
| Quickstart      | [histograph/quickstart](https://github.com/histograph/quickstart)           | Quick start scripts for Histograph
| PITs to GeoJSON | [histograph/pits-to-geojson](https://github.com/histograph/pits-to-geojson) | Convert PIT NDJSON to GeoJSON file
| Reasoner        | [histograph/reasoner](https://github.com/histograph/reasoner)               | Finds matching PITs from different datasets and creates links between them
| Relationizer    | [histograph/relationizer](https://github.com/histograph/relationizer)       | Web interface to find PITs and easily create relations between them
| Stats viewer    | [histograph/stats-viewer](https://github.com/histograph/stats-viewer)       | Visualizations for JSON results of stats module
| Cypher examples | [histograph/cypher-examples](https://github.com/histograph/cypher-examples) | Cypher query examples

## License

Copyright (C) 2015 [Waag Society](http://waag.org).

The source for Histograph is released under the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
