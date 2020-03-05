helm upgrade --install example ./mychart -f ./mychart/domainlist.yaml --set service.type=LoadBalancer

helm upgrade --install example ./mychart -f ./mychart/domainlist.yaml --set service.type=LoadBalancer --set deployments.servicelist[1].image=prasenjit/company-service:v1


while [ true ]; do   curl http://35.225.69.104/; done

helm history example

helm rollback example 1
