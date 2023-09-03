# akuity-appofapps

# validate minikube
minikube start --cpus 8 --memory 16g --container-runtime containerd 

## debug istio
kubectl label namespace default istio-injection=enabled
kubectl label namespace microservices istio-injection=enabled


kubectl apply -f https://raw.githubusercontent.com/istio/istio/release-1.18/samples/bookinfo/platform/kube/bookinfo.yaml
