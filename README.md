# solr-nutch-orchestrator

Launch fast and easy  an Apache Solr linked with Apache Nutch in separated docker containers.

## Usage

First we must configure the several options from nutch/conf and solr/conf.

Then we need to build the two images:

```
docker build -t solr solr/
docker build -t nutch nutch/
```

### Launch Solr

```
docker run -d -p 8983:8983 --name solr solr
```

### Launch nutch

```
docker run -i -t --name nutch --link solr nutch
```