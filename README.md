<h1 align="center">Deploy A Front & Backend App on Kubernetes</h1>

<p >Project Description: Deploy an end-to-end application using MongoDB and Mongo Express on Kubernetes</p>

## Links

- [Repo](https://github.com/raysylverne/mongodb_app "<mongo-app> Repo")

## Screenshots
<img width="1022" alt="8" src="https://user-images.githubusercontent.com/111945210/218289833-7882a758-c362-407b-a758-edc8a9a3187b.png">

<img width="1167" alt="9" src="https://user-images.githubusercontent.com/111945210/218289780-6b52a01b-db77-4439-9ff8-8c26e9bd5d2b.png">


## Commands

### install hyperhit and minikube
`brew update`

`brew install hyperkit`

`brew install minikube`

`kubectl`

`minikube`

### create minikube cluster
`minikube start --vm-driver=hyperkit`

`kubectl get nodes`

`minikube status`

`kubectl version`

### delete cluster and restart in debug mode
`minikube delete`

`minikube start --vm-driver=hyperkit`

`minikube status`

### kubectl commands
`kubectl get nodes`

`kubectl get pod`

`kubectl get services`

`kubectl create deployment nginx-depl --image=nginx`

`kubectl get deployment`

`kubectl get replicaset`

### debugging
`kubectl logs {pod-name}`

`kubectl exec -it {pod-name} -- bin/bash`

### create mongo deployment
`kubectl create deployment mongo-depl --image=mongo`

`kubectl logs mongo-depl-{pod-name}`

`kubectl describe pod mongo-depl-{pod-name}`

### delete deplyoment
`kubectl delete deployment mongo-depl`

`kubectl delete deployment nginx-depl`

### create or edit config file
`vim nginx-deployment.yaml`

`kubectl apply -f nginx-deployment.yaml`

`kubectl get pod`

`kubectl get deployment`

### delete with config
`kubectl delete -f nginx-deployment.yaml`

#Metrics

`kubectl top` The kubectl top command returns current CPU and memory usage for a cluster’s pods or nodes, or for a particular pod or node if specified.

## Future Updates

- [ ] Adding a website

## Author

**Raymond Sylverne**

- [Profile](https://github.com/raysylverne "Raymond Sylverne")
- [Email](mailto:raysylverne@gmail.com?subject=Hi "Hi!")
- [Website](https://medium.com/@RaySylverne "Welcome")
- [LinkedIn](https://www.linkedin.com/in/ray-sylverne/)

## 🤝 Support

Contributions, issues, and feature requests are welcome!

Give a ⭐️ if you like this project!
