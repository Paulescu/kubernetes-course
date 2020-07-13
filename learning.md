eval $(minikube docker-env)
eval $(docker-machine env -u)

kubectl get all

kubectl apply -f <first-pod.yaml>

kubectl describe pod webapp

kubectl exec webapp ls

https://gist.github.com/kevin-smets/b91a34cea662d0c523968472a81788f7

kubectl rollout status deployment webapp 