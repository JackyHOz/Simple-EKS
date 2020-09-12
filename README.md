Install eksctl and kubectl

Please follow this link to config some setting

(Start the workshop and Launch using eksctl)

https://www.eksworkshop.com/


Please replace some content in backend.yaml

image: ""#"your image link"

containerPort: 80#image port number


Run Command

kubectl apply -f eksworkshop.yaml  

kubectl apply -f backend.yaml

kubectl apply -f service.yaml 

kubectl apply -f frontend.yaml

Get External IP

kubectl get service frontend --watch


Scaling

change number in backend.yaml

(replicas: 2)

save and run command:

kubectl apply -f backend.yaml


Reference Link 

https://kubernetes.io/docs/tasks/access-application-cluster/connecting-frontend-backend/

https://www.eksworkshop.com/
