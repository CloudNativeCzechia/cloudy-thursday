# CI/CD/CR
#show #cncz #notes

## What is the show about
Todays topic is real stories from Continuous Integration / Development / Release.

## What is CI/CD/CR
Technically: tooling that enables to run various tooling on defined events (commit, pr, merge, cron). Tooling comprises e.g. testing, syntactic checks, static code analysis, packaging, distribution of the code, deployment of the code.

Mentaly: It is a way of thinking and working. It is not just set of tools, it is the whole way of developing applications. When going continuous, methods how one develops applications have to change. Everything have to be prepared for automation: auto failures, auto rollbacks, testing and system how to discover bugs before depployment and how to rollback production fast to one step back.

Implementing the CI/CD/CR ideas requires significant investments.

## Tools

Pipeline, Runner, Artifact Registry (images, packages, ...).

## Public cloud
AWS: https://aws.amazon.com/getting-started/projects/set-up-ci-cd-pipeline/, https://aws.amazon.com/devops/
Azure: https://azure.microsoft.com/en-us/services/devops/?nav=min 

### SaaS
Jenkins: https://www.jenkins.io/ oldie but goldie, still offers a lot of functionality, a lot of existing workloads are still running it
Gitlab: https://about.gitlab.com/ 
Github: https://github.com/features/actions 
CircleCI: https://circleci.com/ 
Travis: https://travis-ci.org/ 

### Kubernetes
Tekton: https://tekton.dev/
Jenkins-x: https://jenkins-x.io/ 
Agro: https://argoproj.github.io/
Spinnaker: https://spinnaker.io/

## Timeline

- build, release, run  
- release strategies  
- DB migrations in CI  
- GitOps  
- Container-native vs VM-based CI  
- reproducible builds

## Best practices

Automate what is painful for you and you are doing it repeatedly.
Automate what can cause pain, take away the human factor.
Everyone on the team should be aware of the blocks running in the background (not required to understand, but be aware).
The tests are requirement. You are writing the tests for make sure that old code is still working.
You can test in production using canary
Be prepared to rollback.
You have to understand the concept of when to use what method of release: blue - green, canary, continuous rollout, a/b testing. It is not one fit for all uses.
When you build and run, think really hard if the change will wake you up in the 2am when it breaks.
