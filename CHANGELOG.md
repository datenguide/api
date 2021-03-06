# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [0.4.0] - 2020-03-26

## Added

- Initial version of a Graphql wrapper of the GenesAPI Tabular API.

### Changed

- Measures that appear in more than one statistic will include the merged set of all dimensions across
  all statistics.

## [0.3.0] - 2019-12-02

### Changed

- Updated to new structure of Genesapi info.json

## [0.2.0] - 2019-11-29

### Added

- `statisticsCatalog` and `measuresCatalog` GraphQL queries to inspect and query the data schema
- The server now downloads `info.json` on startup and imports the latest schema from GenesAPI `schema.json` and `names.json` instead of previously bundled and static files
- Query and Schema tests

### Security

- CORS middleware to restrict CORS origins

## [0.1.0] - 2019-10-29

### Added

- Initial implementation of the Datenguide API server
- `region` and `allRegions` GraphQL queries
- Experimental complex filter arguments based on [sift](https://github.com/crcn/sift.js) filter syntax.
- GraphQL Playground and GraphiQL Web UIs for interactive GraphQL queries
- HTML homepage for API server

[unreleased]: https://github.com/datenguide/datenguide-api/compare/v0.3.0...HEAD
[0.3.0]: https://github.com/datenguide/datenguide-api/releases/tas/v0.3.0
[0.2.0]: https://github.com/datenguide/datenguide-api/releases/tag/v0.2.0
[0.1.0]: https://github.com/datenguide/datenguide-api/releases/tag/v0.1.0
