---
title: Multicloud incident response navigator
layout: post
author: Jane Hsieh
categories:
  - projects
  - kubernetes
summary: Terminal application designed for operators
thumbnail: posts/anomaly_mode.png
---


Initially named Skipper, the Multicloud incidence response navigator is now an open sourced, interactive terminal tool for managing multiple kubernetes clusters, potentially from different cloud providers.

With the goal of helping operators manage multi-cluster applications with Kubernetes, the Skipper team set up to unravel the some of the most frequent and bothersome painpoints via multiple rounds of user interviews with operators and users in various positions.

Based on the interview results, some of the most common painpoints included:

1. Forgetting the current context when triaging or looking for a resource (especially namespaces and clusters)
2. Having to navigate multiple dashboards to identify anomalous resources and monitor traffic
3. Not understanding the relationships between resources

Inspired by these findings, we employed an intuitive tree-style navigational structure that displays resources and reveals the hierarchical structures of resources, right in the terminal.

On the left pane, four modes exists  for navigation: cluster, application, anomaly and query modes. These allow the user to investigate the cluster and application infrastructures, quickly locate anomalous resources as well as to filter and search for specific resources.



On the right, we also have 4 types of information to display about resources: a customized summary that including crucial information as well as a usage report provided by Prometheus, the yaml file that was applied to create the resource, logs, as well as a table of recent events.



- [Check out Skipper on Github](https://github.com/IBM/multicloud-incident-response-navigator)
