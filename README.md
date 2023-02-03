# Node Test Infrastructure
This repository is for studying k8s and how I can implement more things about it.

> ### Setting up 
To run this you need at least a minikube cluster installed and running.

```sh
kubectl apply -f deployment.yaml -f nginx.yaml
```

Then after a seconds, you can use [k9s](https://github.com/derailed/k9s) to open and monitore your pods. To check if all is good you can open your browser with `minikube service node-test-infra` (if you have minikube) and open `/` or `/nginx`. If you have another cluster you can get the external IP using `kubectl get svc`, where is node-test-infra external's IP.
