# Kubernetes

The `20s` section contain examlples, instructions, scripts, for Kubernetes general and cloud-provider specific use cases. 
To minimize repetitive and irrelevant information, this section makes use of [kustomize](https://kustomize.io/). Each level in this section builds on top of the others with `20-kubernetes/01-standalone` as the base. Though it is not necessary, for effective use of the exampmles it is recommended to be familiar with concepts such as "resources" and "patches" in `kustomize`. 

First, install kustomize: `brew install kustomize`. Then, to simply view what is happening in each directory, run commands like `kustomize build <path/to/directory> > output.yaml`. Example, for "fullstack": `kustomize build ./20-kubernetes/02-fullstack > ./output.yaml`

This section is broken up as follows: 

## 20-kubernetes
General use examples - These examples focus on deploying the products without considering the surrounding infrastructure. 

### 01-standalone
Focus on a baseline deployment for each product. Leverages the `getting-started` profile to provide a vanilla, standalone instance. 

### 02-fullstack
Improves on the deployment from 01-standalone by using the `baseline` profile. This profile provides a simple use case and all of the products integrated together.


