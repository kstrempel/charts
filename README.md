# Helm charts that I missed

### Add this repro to your local helm installation

`helm repo add kstrempel https://kstrempel.github.io/charts/repo/stable`

### Install fake SQS into into you developer kubernetes machine

`helm install --name fake-sqs kstrempel/fake-sqs`

Proxy forword the the pod to make it available outside of k8s.

`kubectl port-forward fake-sqs-<pod-name> 4568:4568`