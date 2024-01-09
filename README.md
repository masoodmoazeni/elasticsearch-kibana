# elasticsearch-kibana



chmod 777 -R els

sudo sysctl -w vm.max_map_count=262144


add upper command in systemd

https://askubuntu.com/questions/919054/how-do-i-run-a-single-command-at-startup-using-systemd



```PUT /elastic_visiton_product```

```GET elastic_visiton_product/_doc/10970```

command curl for create index
```
curl -X PUT "url:9200/elastic_visiton_product"
```

```
GET elastic_visiton_product/_doc/_search
{
    "query": {
        "match_phrase": {
            "title": "نرگس لیمو"
        }
    }
}
```

```
DELETE elastic_visiton_advertise
```
for best search in elastic
```
https://stackoverflow.com/questions/31176000/like-search-in-elasticsearch
```

```
https://www.elastic.co/guide/en/elasticsearch/client/php-api/current/updating_documents.html
```

```
https://depot.dev/blog/docker-clear-cache

https://tech.forums.softwareag.com/t/how-to-clear-docker-cache/283214
```

```
https://stackoverflow.com/questions/50609417/elasticsearch-error-cluster-block-exception-forbidden-12-index-read-only-all
```

```

PUT _cluster/settings
{
  "transient": {
    "cluster.routing.allocation.disk.watermark.low": "100gb",
    "cluster.routing.allocation.disk.watermark.high": "50gb",
    "cluster.routing.allocation.disk.watermark.flood_stage": "20gb",
    "cluster.info.update.interval": "1m"
  }
}
GET /_cat/nodes?v&h=id,diskTotal,diskUsed,diskAvail,diskUsedPercent
POST /elastic_visiton_advertise,elastic_visiton_product/_cache/clear
POST /_cache/clear

PUT _settings
    {
    "index": {
    "blocks": {
    "read_only_allow_delete": "false"
    }
    }
    }

PUT .kibana/_settings
{
"index": {
"blocks": {
"read_only_allow_delete": "false"
}
}
}
```
