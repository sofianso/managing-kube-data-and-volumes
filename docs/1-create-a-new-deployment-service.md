## Build the image
`docker build -t sofianso/kube-data-demo .`

## Push to Docker hub
`docker push sofianso/kube-data-demo`

## Start Minikube
`minikube start --driver=virtualbox`

## Apply Service And Deployment
`kubectl apply -f=service.yaml -f=deployment.yaml`

## Check Running Deployments
`kubectl get deployments`

## Expose The Service
`minikube service story-service`

## What's Next
You can now use the URL from exposing the service to `POST` or `GET` data.
For example: URL will be different but you can paste the link -> `http://192.168.59.100:31382/story` in Postman to `POST` or `GET` data..