---
title: "GKE Auto Pilot"
categories:
  - GoogleCloud
  - Initial
tags:
  - GoogleCloud
  - read more
  - layout
#header:
# overlay_image: /assets/images/pexels-aleksandar-pasaric-325185.jpg
#    #caption: "Photo by [Joel Filipe](https://unsplash.com/@joelfilip) on [Unsplash](https://unsplash.com)"
classes: wide
---

<p align="center">
  <img width="660" height="100" src="/assets/images/Autopilot.png">
</p>

# Google Auto Pilot


Kubernetes is an open-source container-orchestration system for automating computer application deployment, scaling, and management of micro-service applications. The k8 has enabled the organizations to run the containers and the microservices based architectures with ease. But what about the ease of managing the K8 Cluster? Organizations must go through a steep curve associated with moving to microservices and containers. Scaling the Kubernetes cluster, the complexity of managing the control plane, management of the nodes , the API layer are some of the challenging tasks of maintaining the K8. For the organizations it would make more sense to invest in their time in the development and innovation in building the microservices of their business functions rather than spending time on the management of the like the K8 clusters. One way to achieve this is to move to a managed Kubernetes cluster. From the perspective of the public clouds, there are several Kubernetes services like GKE, EKS or AKS. All these services made the deployment of Kubernetes services easy, but each has its own pro's and con's. Each of these services abstracts the control plane from view and you do not need to worry about maintaining the Kubernetes state. It allows you to not worry about maintaining Kubernetes state or its API. Each managed service abstracts the control plane from view.

Google Kubernetes Engine (GKE) provides a managed environment for deploying, managing, and scaling your containerized applications using Google infrastructure. The GKE environment consists of multiple machines grouped together to form a cluster. When you run a GKE cluster, you get the benefit of advanced cluster management features that Google Cloud provides like the load-balancing, automatic scaling, automatic upgrades of the node software, logging and monitoring among others. You would still need to perform a lot of management like to determine the configurations needed for your production workloads, provision the resources, monitor the health of your nodes, calculate the amount of compute capacity that your workloads require. This would take up considerable amount of time an Kubernetes admin's work.

Some of these manual tasks of managing the GKE can be automated by using a new mode of GKE operation called as the "Auto pilot".Autopilot is a new mode of operation in Google Kubernetes Engine (GKE) that is designed to reduce the operational cost of managing clusters, optimize your clusters for production, and yield higher workload availability. The mode of operation refers to the level of flexibility, responsibility, and control that you have over your cluster. With Autopilot, you no longer have to monitor the health of your nodes or calculate the amount of compute capacity that your workloads require. Autopilot supports most Kubernetes APIs, tools, and its rich ecosystem. You stay within GKE without having to interact with the Compute Engine APIs, CLIs, or UI, as the nodes are not accessible through Compute Engine, like they are in Standard mode. You pay only for the CPU, memory, and storage that your Pods request while they are running. Autopilot clusters are pre-configured with an optimized cluster configuration that is ready for production workloads. This streamlined configuration follows GKE best practices and recommendations for cluster and workload setup and security. Some of these built-in settings are immutable and other optional settings can be turned on or off.

In the next blogs I will try to touch upon some of the constraints of moving to the GKE Autopilot, comparing the default and Autopilot mode of operation, Workload limitations and restrictions among other points.
