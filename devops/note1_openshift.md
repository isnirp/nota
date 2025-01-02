# openshift
- A container orchestration platform that works with K8s under the hood.
- origin k8s distribution

## how it works (rough overview)
- dev pushes code to a repo
- jenkins builds and creates an image
- the image is pushed to an artifactory (private/public)
- the container is then pushed to the openshift(k8s) cluster

## openshift vs k8s