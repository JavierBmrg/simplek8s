Tipical commands

- Start k8s cluster  
  `minikube start`

- Know cluster status  
  `minikube cluster-status`

- Show cluster IP  
  `minikube ip`

- Start a Pod Object  
  `kubectl apply -f <pod-path>.yaml`

- Show Pods info  
  `kubectl get pods`

- Show services info  
  `kubectl get services`

- Show more details about a Pod  
  `kubectl describe pod <pod-name>`

- Show deployments objects  
  `kubectl get deployments`

- Re-pull containers in order to update Deployments/Pods (Imperative)
  `kubectl set image <object-type>/<object-name> <container-name> = <new image to use>`
  example: `kubectl set image deployment/client-deployment client=ewfnz/react-nginx-client:v1`

## Flow

- Build a new image and set a tag.
- Push the image to Container Repository
- Use the image(s) for deployments/pods
