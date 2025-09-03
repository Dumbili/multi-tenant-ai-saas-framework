# Multi-Tenant SaaS AI Platform - Dissertation Implementation


This repository contains the practical artefacts and implementation code for my MSc dissertation: **"Building a Multi-Tenant SaaS AI Platform: Design Patterns and Deployment Strategies"**.

## Overview

This project implements a cloud-native isolation framework for multi-tenant AI workloads using Kubernetes. It demonstrates logical tenant separation using namespaces, performance isolation via resource quotas, and secure deployment practices.

## Repository Structure
├── manifests/ # Kubernetes YAML deployment files
├── evidence/ # Screenshots and outputs from testing platforms
└── README.md # This file


## How to Deploy

1.  Ensure you have `kubectl` configured to point to a Kubernetes cluster.
2.  Clone this repository: `git clone <your-repo-url>`
3.  Navigate to the manifests directory: `cd manifests`
4.  Run the deployment script: `./deploy.sh`
    *Or apply manifests manually:*
    `kubectl apply -f 01-namespaces.yaml`
    `kubectl apply -f 02-resource-quotas.yaml`
    `kubectl apply -f 03-deployments.yaml`
    `kubectl apply -f 04-services.yaml`

## Validation Evidence

Screenshots from the implementation and testing on two independent platforms (KillerCoda and LabEx) are provided in the `/evidence` directory, demonstrating the portability and consistency of the declarative deployment approach.

