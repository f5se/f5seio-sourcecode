---
title: "CNI Tools"
date: 2022-11-18T8:51:13+08:00
draft: false
hideLastModified: true
keepImageRatio: yes
summaryImage: "cni-tools.png"
tags: ["cni", "k8s", "flannel", "calico", "cilium"]
summary: "The tools used to setup CNI integration between BIG-IP and Kubernetes."
showInMenu: false
---

BIG-IP as the powerful ADC provider can works only in tranditional data centers but also modern cloud environments, for example, integrating with K8S.

This is a project providing tools used to setup CNI integration between BIG-IP and Kubernetes.

[BIG-IP Kubernetes Gateway API Controller](https://github.com/f5devcentral/bigip-kubernetes-gateway) is using it for initial CNI setup. Surely that, [CIS](https://github.com/F5Networks/k8s-bigip-ctlr) and [CIS-C](https://cis-c.f5se.io/) can, too.

Supported CNIs: Flannel and Calico.

Refer to the [code repository](https://github.com/f5devcentral/cni-tools/) for usage.
