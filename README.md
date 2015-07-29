# Histograph

Historical geocoder, built with [Neo4j](http://neo4j.com/) and [Elasticsearch](https://www.elastic.co/products/elasticsearch). See [histograph.io](http://histograph.io/) or the GitHub repositories of one of the components for more information.

## Components

| Name         | GitHub                                                                | Description
|:-------------|:----------------------------------------------------------------------|:-------------------------------------------------------------
| Core         | [histograph/core](https://github.com/histograph/core)                 | Consumes Redis queue and syncs Neo4j and Elasticsearch
| API          | [histograph/api](https://github.com/histograph/api)                   | Search and dataset API
| Schemas      | [histograph/schemas](https://github.com/histograph/schemas)           | Ontology and [JSON schemas](http://json-schema.org/)
| Config       | [histograph/config](https://github.com/histograph/config)             | Configuration files
| Neo4j Plugin | [histograph/neo4j-plugin](https://github.com/histograph/neo4j-plugin) | Server plugin for Neo4j for certain graph queries
| Viewer       | [histograph/viewer](https://github.com/histograph/viewer)             | Map viewer, [React](http://facebook.github.io/react/) + [Leaflet](http://leafletjs.com/) + [D3.js](http://d3js.org/)
| Data         | [histograph/data](https://github.com/histograph/data)                 | Scripts to download and generate Histograph datasets from selection of sources
| Import       | [histograph/import](https://github.com/histograph/import)             | Scripts to import data into Histograph API

## License

Copyright (C) 2015 [Waag Society](http://waag.org).

The source for Histograph is released under the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
