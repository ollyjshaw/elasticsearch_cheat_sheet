# elasticsearch_cheat_sheet
Some commands I find useful

###Search an index
POST 127.0.0.1:9200/pages/_search
```json
{    "query": {
        "query_string": {
            "query": "foo"
        }
    }
}
```
