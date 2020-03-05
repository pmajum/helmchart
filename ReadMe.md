helm init --service-account tiller --history-max 200

kubectl apply -f tiller-sa.yaml

helm upgrade --install example ./mychart -f ./mychart/domainlist.yaml --set service.type=LoadBalancer

helm upgrade --install example ./mychart -f ./mychart/domainlist.yaml --set service.type=LoadBalancer --set deployments.servicelist[1].image=prasenjit/company-service:v1

With Creating namespace:
helm upgrade --install example ./mychart -f ./mychart/domainlist.yaml --namespace test --set service.type=LoadBalancer


while [ true ]; do   curl http://35.225.69.104/; done

helm history example

helm rollback example 1
