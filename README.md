### How to run this app

0. Install minikube and prereqs from this link: https://minikube.sigs.k8s.io/docs/start/
1. Create a minikube cluster locally: `minikube start`
2. Apply the kubernetes manifest file in the directory: `kubectl apply -f ./`
3. Make sure that the nodeport service is running: `kubectl get services`
4. Make sure that the service pod is running: `kubectl get pods`
5. OPTION 1: Access the service using a tunnel: `minikube service tamatem-takehome`
6. OPTION 2: Access the service using manual port forwarding: `kubectl port-forward service/tamatem-takehome [any-port]:80`
