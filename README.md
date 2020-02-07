git clone https://github.com/neotkm/k8s_demo  

pod-test.yaml - описание контейнера  
svc-test.yaml - описание сервиса  
ingress-test.yaml - описание ингресса  

kubectl apply -f pod-test.yaml -f svc-test.yaml -f ingress-test.yaml  

kubectl get po  
kubectl get ing  
kubectl get svc 
kubectl get ep  



---
kubectl create ns test  
kubectl apply -f pod-read-create-role.yaml  
kubectl apply -f pod-read-create-rb.yaml  


kubectl auth can-i get po --namespace test --as jsalmeron  
kubectl auth can-i get po --namespace kube-system --as jsalmeron  
kubectl auth can-i delete po --namespace kube-system --as jsalmeron  
kubectl auth can-i delete po --namespace test --as jsalmeron  


http://localhost:8001/api/v1/namespaces/kube-systems/services/https:kubernetes-dashboard:/proxy/#/secret?namespace=_all  




