# verdaccio-setup
Verdaccio and nginx setup using docker 


for kibana 
after docker-compose up -d


docker exec -it elasticsearch /usr/share/elasticsearch/bin elasticsearch-create-enrollment-token -s kibana

docker exec -it elasticsearch /usr/share/elasticsearch/bin/elasticsearch-reset-password -u elastic

openssl s_client -connect http://0.0.0.0:9200