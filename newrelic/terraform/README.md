# Terraform

This Terraform deployment is prepared in order to achieve instant observability after deploying Prometheus. It will deploy a dashboard with the following pages:

1. Node Overview
2. Namespace Overview
3. Pod Overview

An example bash script to perform the Terraform deployment can be found [here](../../scripts/02_deploy_newrelic_terraform.sh).

## Node Overview

In order to be able to visualize this page properly, the Prometheus will going to need rights to scrape the following resources:
* Nodes Endpoints
* Node Exporter
* Kube State Metrics

![Node Overview](../../docs/node_overview.png)

## Namespace Overview

In order to be able to visualize this page properly, the Prometheus will going to need rights to scrape the following resources:
* Node cAdvisor
* Kube State Metrics

![Namespace Overview](../../docs/namespace_overview.png)

## Pod Overview

In order to be able to visualize this page properly, the Prometheus will going to need rights to scrape the following resources:
* Node cAdvisor
* Kube State Metrics

![Pod Overview](../../docs/pod_overview.png)
