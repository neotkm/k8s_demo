pod-test.yaml - описание контейнера  
svc-test.yaml - описание сервиса  
ingress-test.yaml - описание ингресса  

kubectl apply -f pod-test.yaml -f svc-test.yaml -f ingress-test.yaml  

kubectl get po  
kubectl get ing  
kubectl get svc 
kubectl get ep  



