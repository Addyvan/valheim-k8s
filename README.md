# valheim-k8s

Basic kubernetes deployment valheim on a k8s homelab. Based off the work by lloesche [here](https://github.com/lloesche/valheim-server-docker). 

Quickly made this to play with some friends. I can template this further, respond to gh issues, and make the chart repo available via an index file if there is genuine interest. 

## Current pre-reqs

* A kubernetes cluster 
  * Ability to create LoadBalancer services (using metallb or cloud)

## Usage

```bash
helm install valheim-server ./chart  \
  --set worldName=example-world-name \
  --set serverName=example-server-name \
  --set password=password
```
## Storage

This is current using a `hostPath` volume as it is configured for a bare metal cluster. Please create an issue if you would like support for specific cloud storage solutions via PVCs / storageclasses. They vary by provider so PRs / testers welcome for this. 
