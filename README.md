# DOTT: DevOps Test Task

Welcome to DOTT.

This repository contains an API skeleton where you can add your code,
choose the language of your preference.

## What do we expect from you?

* Demonstrate you have great coding and operation skills, no matter which
technology stack is used.

* This is not an exam, this is more a task that has been assigned to you,
so you can ask us at anything, anytime.

* Communication is important, if you don't have technical problems make sure
to share your progress.

## Application Overview

You need to complete a functionality in our API that provides some help to
the networking team.

The API has 3 missing endpoints, the first endpoint converts Subnet Mast to
CIDR format, the second endpoint return the CIDR value of a given Subnet Mask
and finally the third endpoint simply validates an IPv4.

e.g.

```
curl localhost/cidr-to-mask?value=24
{
  "function": "cidrToMask",
  "input": "24",
  "output": "255.255.255.0"
}
```

```
curl localhost/mask-to-cidr?value=255.255.0.0
{
  "function": "maskToCidr",
  "input": "255.255.0.0",
  "output": "16"
}

```

```
curl localhost/ip-validation?value=255.255.0.0
{
  "function": "ipv4Validation",
  "input": "255.255.0.0",
  "output": true
}

```


## What do you need to do?

### Continuous Integration
  * Define a CI pipeline.
  * The pipelines must be checked in code (Jenkinsfile or Scripts).
  * Automate your tests every time a change is pushed to the repository.
    - Avoid buggy code to be deployed.

### Continuous Delivery

  * Define your CD pipeline.
  * Deploy to your Production Environment based on your defined strategy.
  * Manage stage as production.
  * Deploy to your Testing Environment before deploying to stage or production.
  * Deploy with no downtime in production.
  
### Coding
  * Complete the following endpoints.
   - `/mask-to-cidr?value=<VALUE>`
   - `/cidr-to-mask?value=<VALUE>`
  * The following endpoint is not required for this phase.
   - `/ip-validation?value=<VALUE>`
  * Make sure your tests are passing
  * Add missing tests
  * You should pick one from a list of available languages.
    - [Python](cidr_convert_api/python)
    - [Go](cidr_convert_api/go)
    - [Java](cidr_convert_api/java)
    - [NodeJS](cidr_convert_api/node)
    - [Ruby](cidr_convert_api/ruby)

## Infrastructure Management

  You will have access to the following:

  * AWS EC2 Insance

### How to access the infrastructure:
  * You will be given a dedicated machine for your task. You should recieve the following:
    - IP of the EC2 instance
    - Access keys / .pem file


### Using Docker Builder
  * Docker can be integrated with Jenkins, in a job you could use this
  command to build an image

```
 docker build -t my-image:some-tag .
```

  * You will need to push data to a remote docker registry.
