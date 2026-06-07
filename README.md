# PayPal Demo Application on Kubernetes 🚀

A hands-on Kubernetes deployment project that demonstrates how to deploy and manage a multi-component application using Kubernetes resources and namespaces.

The goal of this project was to gain practical experience with Kubernetes concepts such as Deployments, Services, Namespaces, scaling, and application management.

## Project Overview

The application is deployed inside a dedicated Kubernetes namespace and managed through Kubernetes manifests.

This project demonstrates how containerized applications can be deployed, exposed, and managed within a Kubernetes cluster.

## Kubernetes Components

### Namespace

A dedicated namespace is used to isolate application resources:

* paypal-namespace

### Deployments

Deployments are used to:

* Manage application pods
* Ensure desired replica count
* Support rolling updates
* Provide self-healing capabilities

### Services

Services are configured to:

* Expose application components
* Enable communication between workloads
* Provide stable network endpoints

## Project Structure

```text
paypal-demo/
├── namespace.yaml
├── deployment.yaml
├── service.yaml
├── screenshots/
└── README.md
```

## Technologies Used

* Kubernetes
* Docker
* Minikube
* kubectl
* Linux

## Skills Practiced

* Creating and managing Namespaces
* Deploying applications with Deployments
* Exposing applications with Services
* Scaling workloads
* Monitoring Pods and Deployments
* Troubleshooting Kubernetes resources
* Managing application lifecycle using kubectl

## Common Commands

View Pods:

```bash
kubectl get pods -n paypal-namespace
```

View Services:

```bash
kubectl get svc -n paypal-namespace
```

View Deployments:

```bash
kubectl get deployments -n paypal-namespace
```

Scale Application:

```bash
kubectl scale deployment <deployment-name> --replicas=5 -n paypal-namespace
```

## Learning Outcomes

Through this project, I gained practical experience with:

* Kubernetes architecture and resource management
* Application deployment workflows
* Service discovery and networking
* Scaling and workload management
* Troubleshooting Kubernetes environments

## Future Improvements

* Add Ingress Controller
* Implement ConfigMaps and Secrets
* Add Persistent Volumes
* Integrate CI/CD pipelines
* Deploy on a cloud-hosted Kubernetes cluster

## Author

Ahmed Adel

AIOps Engineer Trainee | DevOps & Cloud Enthusiast
