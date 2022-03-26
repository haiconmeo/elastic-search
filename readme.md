# Deploy
```
    sudo docker-compose.yml up -d
```
# access elasticsearch, kibana
```
    <ip>:5601
```
# install libraries
    pip install -r requirements.txt
## Modify connection to elasticsearch in file elasticsearch_utils.py

```
client = Elasticsearch(host="0.0.0.0", port="9200")
```
# create index
```
    create_index(<name index>)
```
# delete index
```    
    delete_index(<name index>)
```
# search elasticsearch
```
    search_es_ds(<name index>, fields)

    Ex: search_es_ds('demo', [{"_id" : '123'}])
```
