# Helm3

## Setup

1. Create namespace  
`kubectl create namespace softcon-app-helm`

1. Verify Helm charts

```
helm install softcon-app-helm ./softcon-helm -n softcon-app-helm --dry-run
```

1. Install Helm charts

```
helm install softcon-app-helm ./softcon-helm/ -n softcon-app-helm
```
- Don't forget to make sure that the image required for the deployment is in the microk8s repository.
