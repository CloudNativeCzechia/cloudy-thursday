# Cloudy Thursday ep. 1 
###### tags: `show`

## Topic

> The topic for discussion on this episode

Top 5 cloud trends from 2020
[newstack](https://thenewstack.io/the-new-stack-top-cloud-native-technology-trends-from-2020/)


## Introduction

> Every episode have to have this one the same, we do forget about it.

- Who we are
- New Year, New Name
    - So what is new
- How have we been
- Something interesting we are working on / anything really
- Disclaimer everything we say is our opinion
- Repeat the topic what are we going to discuss


## News 

> Was there anything interesting

- @petr: [Azure now allows more langugaes in function with custom handlers](https://techcommunity.microsoft.com/t5/apps-on-azure/azure-functions-in-any-language-with-custom-handlers/ba-p/1942744?WT.mc_id=AZ-MVP-4021705)
- @petr: [5 new free tier services in Azure](https://azure.microsoft.com/en-us/updates/five-more-free-services-now-available-in-the-azure-free-account/)
- @petr: [Azure health bot](https://azure.microsoft.com/en-us/blog/introducing-azure-health-bot-an-evolution-of-microsoft-healthcare-bot-with-new-functionality/)
- @robert: [Amazon ECS Announces the Preview of ECS Deployment Circuit Breaker](https://aws.amazon.com/about-aws/whats-new/2020/12/amazon-ecs-announces-the-preview-of-ecs-deployment-circuit-breaker/)
- @robert: [Run Serverless Kubernetes Pods Using Amazon EKS and AWS Fargate](https://aws.amazon.com/about-aws/whats-new/2019/12/run-serverless-kubernetes-pods-using-amazon-eks-and-aws-fargate/)
- @robert: [Amazon EKS adds support for EC2 Spot Instances in managed node groups](https://aws.amazon.com/about-aws/whats-new/2020/12/amazon-eks-support-ec2-spot-instances-managed-node-groups/)

Azure functions are now simmilar to Google cloud run. 

## Discussion notes

> To refresh our memory on the go


### A Programmable Linux Kernel

eBPF in a linux kernel. Baked in a filter that expanded to enable sandboxed code execution.


### Return of the monolith 

Problems with microservices vs Problems with monoliths.
How to actually tackle this problem? How can I make sense out of it? How to implement?


### Unified K8s control plane

K8s is hard especialy if you want to focus only on application and not on the infra.
Developers does not want to focus on multiple things and they do not have time to figure out
the complexity hidden in the K8s.

Therefore new initative exists to unify the app experience on K8s.

There is Open Application Model https://github.com/oam-dev 

We will return to this one in the next episode.


### Security score rethinking 

An idea how we approach vulnerabilities. It turned out that CVEs with high scores are usually 
patched faster, but have never been loaded into memory, so there were not abused.

Instead attackers used lower scored CVEs to breach the security.


### Rust creeping into system programming and eating C position

Rust is gaining traction as a secure language for low level tasks. It tries to solve all the problems
C/C++ have by making it virtually imposible to write bad code.

I have not tried Rust just yet, but I am puzzled as I have been C/C++ developer for good 7 years.
And definitely did not found it hard. Challenging yes, but not hard to write good code. 
However you have to be skilled and know what are you doing.


## QA

--- 
