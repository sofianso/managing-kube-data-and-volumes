## Rebuilding The Pod
After adding the `./error` block of code in `app.js`, you need to rebuild the pod.

the `1` tag will diffrentiate the docker image

`docker build -t sofianso/kube-data-demo:1 .`

Don't forget to update the image pulled from deployment.yaml to `sofianso/kube-data-demo:1`

Apply the new `deployment.yaml` configuration.
`kubectl apply -f=deployment.yaml`