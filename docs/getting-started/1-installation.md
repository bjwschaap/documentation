---
cover: /LinkedIn_personal_(3).png
title: Installation
description: Getting started with installing Memphis.dev
---
# Step 1 - Installation

## What is Memphis.dev?

**Memphis.dev** is a next-generation alternative to traditional Message brokers.

It enables building modern queue-based applications that require large volumes of streamed and enriched data, modern protocols, zero ops, up to x9 faster development, up to x46 fewer costs, and significantly lower dev time for data-oriented developers and data engineers.

Low footprint, highly resilient, cloud-native, and run on any Kubernetes, on any cloud.

**Memphis focuses on four pillars -**

1. Reliability - Queues and brokers are a mission-critical component in the modern application architecture and should be highly available and stable as possible.
2. Performance and Efficiency - Provide great performance while maintaining efficient resource consumption.
3. Developer Experience - Enable rapid development and ultra-short time-to-production.
4. Observability - Increase observability, integrations with 3rd-party monitoring tools, real-time notifications, stream lineage, and therefore troubleshooting time reduction.

## **Quick Start**

### **Kubernetes**

Stable -

```bash:line-numbers
helm repo add memphis https://k8s.memphis.dev/charts/ --force-update && 
helm install memphis memphis/memphis --create-namespace --namespace memphis --wait
```

Latest -
```bash
helm repo add memphis https://k8s.memphis.dev/charts/ --force-update
helm install --set memphis.image="memphisos/memphis:latest" memphis memphis/memphis --create-namespace --namespace memphis --wait
```

More information can be found in the [Memphis k8s deployment](/deployment/kubernetes/) documentation.

### **Docker compose (Syntax for v2)**

Stable -&#x20;

```bash
curl -s https://memphisdev.github.io/memphis-docker/docker-compose.yml -o docker-compose.yml && docker compose -f docker-compose.yml -p memphis up
```
Latest -

```bash
curl -s https://memphisdev.github.io/memphis-docker/docker-compose-latest.yml -o docker-compose-latest.yml && docker compose -f docker-compose-latest.yml -p memphis up
```

More information can be found in the [Memphis Docker deployment](/deployment/docker-compose) documentation.

## Walkthrough

<iframe src="https://app.storylane.io/share/upo0paxdvynz" allow="fullscreen" style="border: none;"></iframe>

## High-level diagram

<figure><img src="/assets/overview_(1).jpeg" alt=""><figcaption></figcaption></figure>

