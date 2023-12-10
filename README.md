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
