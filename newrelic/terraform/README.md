# Terraform

This Terraform deployment is prepared in order to achieve instant observability after deploying Prometheus. It will deploy a dashboard with the following pages:

2. [Node overview](../../docs/node_overview.png)
3. [Namespace overview](../../docs/namespace_overview.png)
4. [Pod overview](../../docs/pod_overview.png)

An example bash script to perform the Terraform deployment can be found [here](../../scripts/02_deploy_newrelic_terraform.sh).

## Node Overview

In order to be able to visualize this page properly, the Prometheus will going to need rights to scrape the following resources:
* Nodes Endpoints
* Node Exporter
* Kube State Metrics

## Namespace Overview

In order to be able to visualize this page properly, the Prometheus will going to need rights to scrape the following resources:
* Node cAdvisor
* Kube State Metrics

## Pod Overview

In order to be able to visualize this page properly, the Prometheus will going to need rights to scrape the following resources:
* Node cAdvisor
* Kube State Metrics
