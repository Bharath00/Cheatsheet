Simple Nginx deployment using Kubernetes and Minikube


Required: Docker, Kubernetes, kubectl, minikube

For Kubectl - https://kubernetes.io/docs/tasks/tools/ 
For Minikube - https://minikube.sigs.k8s.io/docs/start/ 

Check if minikube is up and running by using "minikube status" if not then start minikube by using "minikube start"

Note: Services of type LoadBalancer can be exposed via the "minikube tunnel" command. It must be run in a separate terminal window to keep the LoadBalancer running (https://minikube.sigs.k8s.io/docs/handbook/accessing/)

kubectl apply -f <filename>

kubectl get svc <service_name>
* note that without minikube tunnel, kubernetes would be showing external IP as “pending”.

http://REPLACE_WITH_EXTERNAL_IP:8080