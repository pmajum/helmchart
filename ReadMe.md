helm init --service-account tiller --history-max 200

kubectl apply -f tiller-sa.yaml

helm upgrade --install example ./mychart -f ./mychart/domainlist.yaml --set service.type=LoadBalancer

helm upgrade --install example ./mychart -f ./mychart/domainlist.yaml --set service.type=LoadBalancer --set deployments.servicelist[1].image=prasenjit/company-service:v1

With Creating namespace:
helm upgrade --install example ./mychart -f ./mychart/domainlist.yaml --namespace test --set service.type=LoadBalancer


while [ true ]; do   curl http://35.225.69.104/; done

helm history example

helm rollback example 1



############################################################################

./helm upgrade --install normaldeploy ./helmchart/mychart -f ./helmchart/mychart/domainlist.yaml --namespace normaldeploy --set service.type=NodePort

kubectl label node whf00mjp normaldeploy=true

kubectl label node whf00mhy normaldeploy=true

 kubectl get nodes -l normaldeploy=true
 
 kubectl label node whf00mjp normaldeploy-


./helm history normaldeploy -n normaldeploy

 ./helm rollback normaldeploy 8 -n normaldeploy
 
 ./helm delete normaldeploy -n normaldeploy 
 
 
 ./helm get values --revision=3 normaldeploy -n normaldeploy
 
 docker run -d arunvelsriram/utils sleep 1000
 
 




while [ true ]; do   curl http://whf00dit.in.oracle.com:30114/; sleep 1;done
