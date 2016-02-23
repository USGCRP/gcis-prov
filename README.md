# facetview-prov-es
Advanced FacetView User Interface and REST Service for PROV-ES


## Install template

```
cd scripts
./install_es_template.sh http://localhost:9200 prov_es ../config/es_template-prov_es.json
```


## Install

```
cd ..
python setup.py install
```


## Run PROV-ES FacetView on port 8888

```
PROVES_ENV=prod ./manage.py server -h 0.0.0.0 -p 8888
```


## import PROV-ES JSON via curl

```
curl -F "prov_es=<prov_es.json" http://192.168.56.101:8888/api/v0.1/prov_es/import/json
```


## Demo

https://gcis-search-stage.jpl.net/provenance
