# Introduction

Kubernetes is an open source orchestrator for deploying containerized applications.

Benefits:

* Velocity
  - speed => develop => deploy new features
  - constant uptime
    - immutability
    - declarative configuration
    - online self-healing systems
* Scaling
* Abstracting infrastructure
* Efficiency

## Velocity

### Immutability

Scenario 1: Log into container => download new software => kill old server => start new server.

Scenario 2: build new container image => push new container to container registry => kill the existing container => start a new one.

### Declarative configuration

Declarative configuration describes the state of the world => no need to be executed to be understood.

### Self-healing systems

Kubernetes continuously takes actions to ensure that the current state matches the desired state.

## Scaling your service and your teams

Scalability => decoupled architectures.

### Decoupling

* Defined APIs.
  - implementer / consumer
* Load balancers
  - running instances

=> smaller microservice => comprehensible surface area.

### Scaling development teams with microservices

* Pods: group of containers - group container images developed by different teams into a single deployable unit.
* Load balancing, naming, and discovery - isolate one microservice from another
* Namespaces - provide isolation and access control.
* Ingress - frontend - combine multiple microservices into a single externalized API surface area.
