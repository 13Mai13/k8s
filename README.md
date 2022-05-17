# k8s
k8s hands on notes
## Minikube 

### Installing

The official documentation is available here (https://minikube.sigs.k8s.io/docs/start/)

```
brew install minikube
```

Start docker:

```
minikube start --driver docker
```

If everything was propperly installed:

```
minikube status
```

Should print:

```
minikube
type: Control Plane
host: Running
kubelet: Running
apiserver: Running
kubeconfig: Configured
```

## Kubeclt

### Commands

Display nodes:

```
kubectl get node
```

## Project 

* Docker image of the web-app (https://hub.docker.com/repository/docker/nanajanashia/k8s-demo-app)
* Docker image of mongobd (https://hub.docker.com/_/mongo)
* Kubernetes offical documentation (https://kubernetes.io/docs/home/)
