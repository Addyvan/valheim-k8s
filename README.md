# valheim-k8s

Basic kubernetes deployment valheim on a k8s homelab. Based off the work by lloesche [here](https://github.com/lloesche/valheim-server-docker). 

Quickly made this to play with some friends. I can template this further, respond to gh issues, and make the chart repo available via an index file if there is genuine interest. 

## Pre-reqs

* A kubernetes cluster 
  * Ability to create LoadBalancer services (using metallb or cloud)
