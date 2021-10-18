# OpenSearch
There are two images that are present in DockerHub for opensearch.

> opensearchproject/opensearch:1.1.0
> opensearchproject/opensearch-dashboards:1.1.0

**OpenSearch** is the actual search engine
**OpenSearch Dashboard** is the default visualization tool for opensearch, it is replacement of `kibana` 

## Run Opensearch container
> docker compose up -d

### if Opensearch container failed initiate and throws the following error.
`Elasticsearch: Max virtual memory areas vm.max_map_count [65530] is too low, increase to at least [262144]`

**Try running following command**
open powershell run

> wsl -d docker-desktop

then

> sysctl -w vm.max_map_count=262144
