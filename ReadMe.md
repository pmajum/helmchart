helm upgrade --install example ./mychart -f ./mychart/domainlist.yaml --set service.type=LoadBalancer


while [ true ]; do   curl http://35.225.69.104/; done

helm history example

helm rollback example 1
