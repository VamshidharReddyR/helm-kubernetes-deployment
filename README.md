# Helm Kubernetes Deployment

This repository contains a reusable Helm chart for deploying applications to Kubernetes.

## Overview

The project demonstrates how Helm can be used to package, configure, and deploy Kubernetes workloads using reusable templates and centralized configuration.

## Repository Structure

helm-kubernetes-deployment

charts/
└── myapp/
    ├── Chart.yaml
    ├── values.yaml
    └── templates/
        ├── deployment.yaml
        ├── service.yaml
        ├── ingress.yaml
        ├── configmap.yaml
        ├── hpa.yaml
        └── serviceaccount.yaml

## Features

- Helm Chart Packaging
- Kubernetes Deployment Templates
- Service Configuration
- Ingress Configuration
- ConfigMap Integration
- Horizontal Pod Autoscaler Support
- ServiceAccount Configuration
- Centralized Values Management

## Technologies Used

- Helm
- Kubernetes
- YAML
- Git
- GitHub

## Components

### Deployment

Manages application pod deployments using configurable replica counts and container images.

### Service

Exposes application workloads within the Kubernetes cluster.

### Ingress

Provides external access configuration for applications.

### ConfigMap

Stores application configuration outside container images.

### Horizontal Pod Autoscaler

Automatically scales workloads based on CPU utilization.

### ServiceAccount

Provides workload identity configuration for Kubernetes applications.

## Example Deployment

helm install myapp ./charts/myapp

## Future Enhancements

- Secret Management
- StatefulSet Support
- Pod Disruption Budgets
- Network Policies
- Multi-Environment Values Files
