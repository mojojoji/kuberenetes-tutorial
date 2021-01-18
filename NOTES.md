## Kubernetes Basics

- Orchestration
- Achieve desired state via controllers
- Access via kubeconfig `(~/.kube/config)`

## KubeCTL

- Syntax

### Containers

- [Container Images](https://kubernetes.io/docs/concepts/containers/#container-images)
- [Container runtime](https://kubernetes.io/docs/concepts/containers/#container-runtimes)

### Pods

[Pods docs](https://kubernetes.io/docs/concepts/workloads/pods/)

- Smallest deployable entity
- Contains one or more containers
- [Pod spec](https://kubernetes.io/docs/concepts/workloads/pods/#pod-templates)

### Workloads

#### Types of workloads

[Types of Workloads](https://kubernetes.io/docs/concepts/workloads)

- [Deployment](https://kubernetes.io/docs/concepts/workloads/controllers/deployment/)
- [Statufulsets](https://kubernetes.io/docs/concepts/workloads/controllers/statefulset/)
- [DaemonSets](https://kubernetes.io/docs/concepts/workloads/controllers/daemonset/)
- [Job](https://kubernetes.io/docs/concepts/workloads/controllers/job/)
- [CronJobs](https://kubernetes.io/docs/concepts/workloads/controllers/cron-jobs/)

### Services

- Expose an application in one or more pods
- Pods are created and destroyed and have dynamic names. And IPs of pods keep changing. Cant call it directly. Services give a network identity by giving a internal hostname domain.
- [Service definition](https://kubernetes.io/docs/concepts/services-networking/service/#defining-a-service)

#### Types of services

- [ClusterIP](https://kubernetes.io/docs/concepts/services-networking/service/#publishing-services-service-types)
- [NodePort](https://kubernetes.io/docs/concepts/services-networking/service/#nodeport)
- [LoadBalancer](https://kubernetes.io/docs/concepts/services-networking/service/#loadbalancer)
- [External Name](https://kubernetes.io/docs/concepts/services-networking/service/#externalname)
- [External IP](https://kubernetes.io/docs/concepts/services-networking/service/#external-ips)

### Ingress

- Gives external access
- Does ssl, ssl termination, load balancing, routing etc
- [Docs](https://kubernetes.io/docs/concepts/services-networking/ingress/)
