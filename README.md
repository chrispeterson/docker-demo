# start dev stack
    docker-compose pull
    docker-compose up


# Elastic Search

## To view indexed logs run:

    curl "localhost:9200/_search?pretty" \
      -H 'Content-Type: application/json' \
      -d'{ "query": { "match_all": {} }}'



## To "start fresh", delete the index by running:

    curl -X DELETE "localhost:9200/fluent-bit?pretty"