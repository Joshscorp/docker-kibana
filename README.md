# docker-kibana

This is [Kibana 5.2.2](https://github.com/elastic/kibana) in a minimal 113MB Docker image. Images are tagged by Kibana versions.

[![Docker Repository on Quay.io](https://quay.io/repository/pires/docker-kibana/status "Docker Repository on Quay.io")](https://quay.io/repository/pires/docker-kibana)

## Running

```
docker run --name kibana \
           --detach \
           --publish 5601:5601 \
           -e KIBANA_ES_URL=<elasticsearch url> \
           rollerdigital/docker-kibana:5.2.2
```

You could set `KIBANA_INDEX` env variable to set an index for Kibana's data.
