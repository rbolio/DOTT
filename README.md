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

### CI/CD Pipeline
- [ ] Jenkins
    - [ ] Webhook
- [ ] Sonar Qube
    - [ ] (Plus) Linting
    - [ ] Static Code Analysis
- [ ] Testing
    - [ ] Unit testing
    - [ ] Functional Tesging(plus)
- [ ] (Plus) Docker
- [ ] (Plus) Seguridad
- [ ] (Plus) Fix Code

### Techincal Diagram 
- [ ] Processes
- [ ] Information Flow between different technologies

### Task Organization
- [ ] Kanban (Trello.com)

