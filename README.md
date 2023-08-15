# GKE-K8s

This repository will keep the Google Kubernetes Engine YAML files required to replicate part of Research Project environment.


## GCP

Coming soon...


## Minikube

When running locally apply 

```
kubectl apply -f file_name.yaml -n NAMESPACE
```

Where NAMESPACE is your namespace

to all YAML files you find here.

### Go microservices minikube example 

After running

```
kubectl apply -f go-micro/namespace.yml
kubectl apply -f go-micro
```

Apply:

```
minikube start gateway -n go-micro
```

This operation should be done automatically when deployed to GKE.
URL should be returned. 

To check if everything is okay, visit
http://127.0.0.1:33903/hotels?inDate=2014-03-17&outDate=2014-03-21&lat=37.7749&lon=-122.4194

and some JSON with data should be returned. Minikube might return different port with each call of this start command, remember to update it.

