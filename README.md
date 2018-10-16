# beer-service-k8s

This is a simple Spring Boot app to demonstrate deploying an app to kubernetes using concourse.

## Requirements

* running concourse instance with credhub
* running kubernetes cluster


## Setup

1. Add credentials into credhub

    `credhub set -n concourse/main/github_token --type password -w '<your-token>'`
    
    `credhub set -n concourse/main/docker_login --type user -z <your-username> -w '<your-pass>'`

2. Modify the vars file for your set up