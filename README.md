# kubernetes-on-mac
Install Minikube on MacOS

### Install minikube

```
brew cask install minikube

```

### Set environment for docker daemon

```
eval $(minikube docker-env)

```

### Start k8s

```
minikube start

```

### Open k8s dashboard

```
minikube dashboard

```

### Install test app in k8s

```
kubectl run hello-minikube --image=gcr.io/google_containers/echoserver:1.4 --port=8080
 
kubectl expose deployment hello-minikube --type=NodePort

```

### Check test app

```
http://ip_minikube:8080

```

