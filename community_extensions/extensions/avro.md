---
warning: DO NOT CHANGE THIS MANUALLY, THIS IS GENERATED BY https://github/duckdb/community-extensions repository, check README there
title: avro
excerpt: |
  DuckDB Community Extensions
  Read Apache Avro (TM) files form DuckDB

extension:
  name: avro
  description: Read Apache Avro (TM) files form DuckDB
  version: 1.0.0
  language: C++
  build: cmake
  license: MIT
  excluded_platforms: "wasm_mvp;wasm_eh;wasm_threads;windows_amd64_rtools"

  maintainers:
    - hannes

repo:
  github: hannes/duckdb_avro
  ref: 7facc0badf31c7ec0a249cf47fb97d190550d3f2

docs:
  hello_world: |
    FROM read_avro('some_file.avro');
  extended_description: |
    This extension provides a scan function for Apache Avro files.
    For more information and information regarding usage, limitations and performance, see the [README](https://github.com/hannes/duckdb_avro).

extension_star_count: 7
extension_star_count_pretty: 7
extension_download_count: 56
extension_download_count_pretty: 56
image: '/images/community_extensions/social_preview/preview_community_extension_avro.png'
layout: community_extension_doc
---

### Installing and Loading
```sql
INSTALL {{ page.extension.name }} FROM community;
LOAD {{ page.extension.name }};
```

{% if page.docs.hello_world %}
### Example
```sql
{{ page.docs.hello_world }}```
{% endif %}

{% if page.docs.extended_description %}
### About {{ page.extension.name }}
{{ page.docs.extended_description }}
{% endif %}

### Added Functions

<div class="extension_functions_table"></div>

| function_name | function_type | description | comment | example |
|---------------|---------------|-------------|---------|---------|
| read_avro     | table         |             |         |         |



---
