# elasticsearch_cheat_sheet
Some commands I find useful

###Search an index
POST 127.0.0.1:9200/index_name/_search
```json
{    
    "query": {
        "query_string": {
            "query": "foo"
        }
    }
}
```

###Show current indicies
GET localhost:9200/_cat/indices?v

###Show details of a mapping in an index 
GET localhost:9200/index_name/_mapping/mapping_name
