# DevOps-Tasks

Basic DevOps hands-on tasks for beginners looking to learn the ropes. This is a work in progress and will be updated as we go along.

- [DevOps-Tasks](#devops-tasks)
  - [Pre-requisites](#pre-requisites)
    - [Learning](#learning)
    - [Tools](#tools)
    - [Services](#services)
    - [Extra](#extra)
  - [Task 1: Starting apps](#task-1-starting-apps)
    - [Task 1.1 Docker](#task-11-docker)
    - [Task 1.2 Docker-compose](#task-12-docker-compose)
    - [Task 1.3 Kubernetes](#task-13-kubernetes)
  - [Task 2: Pipelines](#task-2-pipelines)
    - [Task 2.1 Jenkins](#task-21-jenkins)
    - [Task 2.2 Gitlab](#task-22-gitlab)
    - [Task 2.3 Github](#task-23-github)
  - [Task 3: Data Formats](#task-3-data-formats)
    - [Task 3.1 JSON](#task-31-json)
    - [Task 3.2 YAML](#task-32-yaml)
    - [Task 3.3 TOML](#task-33-toml)
    - [Task 3.4 XML](#task-34-xml)
    - [Task 3.5 CSV](#task-35-csv)
    - [Task 3.6 INI](#task-36-ini)
  - [Task 4: Infrastructure as Code](#task-4-infrastructure-as-code)
    - [Task 4.1 Terraform](#task-41-terraform)
    - [Task 4.2 Ansible](#task-42-ansible)
    - [Task 4.3 Pulumi](#task-43-pulumi)
    - [Task 4.4 Puppet](#task-44-puppet)
    - [Task 4.5 Chef](#task-45-chef)
    - [Task 4.6 SaltStack](#task-46-saltstack)
  - [Task 5: Cloud Providers](#task-5-cloud-providers)
    - [Task 5.1 AWS](#task-51-aws)
    - [Task 5.2 Azure](#task-52-azure)
    - [Task 5.3 GCP](#task-53-gcp)
    - [Task 5.4 Oracle](#task-54-oracle)
    - [Task 5.5 Digital Ocean](#task-55-digital-ocean)
    - [Task 5.6 Linode](#task-56-linode)
  - [Questions](#questions)
  - [Terms, buzzwords and more](#terms-buzzwords-and-more)

## Pre-requisites

### Learning

Few important notes on how to research and learn:

- [Google](https://www.google.com) is your best friend. You can find anything you want, including the official documentation.
- [Stackoverflow](https://stackoverflow.com) is your second best friend. There is always someone who had the same problem as you.
- [Youtube](https://www.youtube.com) is your third best friend. There is always a video explaining what you are looking for.
- [Reddit](https://www.reddit.com) is your fourth best friend. There is always a community that can help you.

Also most of the tools have communities in Reddit, Discord, Slack, Glip etc. It is good to join them and ask questions if you are stuck.

A good professional is always up-to date with the latest news and trends. For starters you can use the following websites and channels to keep up:

- [PowerCert](https://www.youtube.com/channel/UCJQJ4GjTiq5lmn8czf8oo0Q)
- [A Cloud Guru](https://www.youtube.com/channel/UCp8lLM2JP_1pv6E0NQ38pqw)
- [TLF](https://www.youtube.com/channel/UCfX55Sx5hEFjoC3cNs6mCUQ)
- [Coding Tech](https://www.youtube.com/channel/UCtxCXg-UvSnTKPOzLH4wJaQ)
- [Crosstalk Solutions](https://www.youtube.com/channel/UCVS6ejD9NLZvjsvhcbiDzjw)
- [ExplainingComputers](https://www.youtube.com/channel/UCbiGcwDWZjz05njNPrJU7jA)
- [Linux For Everyone](https://www.youtube.com/channel/UCd4XwUn2Lure2NHHjukoCwA)
- [The Linux Experiment](https://www.youtube.com/channel/UC5UAwBUum7CPN5buc-_N1Fw)
- [DistroTube](https://www.youtube.com/channel/UCVls1GmFKf6WlTraIb_IaJg)
- [Craft Computing](https://www.youtube.com/channel/UCp3yVOm6A55nx65STpm3tXQ)
- [Gary Explains](https://www.youtube.com/channel/UCRjSO-juFtngAeJGJRMdIZw)
- [Simplilearn](https://www.youtube.com/channel/UCsvqVGtbbyHaMoevxPAq9Fg)
- [CBT Nuggets](https://www.youtube.com/channel/UClIFqsmxnwVNNlsvjH1D1Aw)
- [NCIX Tech Tips](https://www.youtube.com/channel/UCjTCFFq605uuq4YN4VmhkBA)
- [Just me and Open Source](https://www.youtube.com/channel/UC6VkhPuCCwR_kG0GExjoozg)
- [NixieDoesLinux](https://www.youtube.com/channel/UCBE-FO9JUOghSysV9gjTeHw)
- [Amit Nepal](https://www.youtube.com/channel/UCIOlfUXD5wYP_uEemv2_LVg)
- [SysAdminGirl](https://www.youtube.com/channel/UCkIHLaOEtdLpC3JrqR3Bwmw)
- [Coding Tech](https://www.youtube.com/channel/UCtxCXg-UvSnTKPOzLH4wJaQ)
- [Computerphile](https://www.youtube.com/channel/UC9-y-6csu5WGm29I7JiwpnA)
- [GotoConferences](https://www.youtube.com/c/GotoConferences)
- [elithecomputerguy](https://www.youtube.com/user/elithecomputerguy)
- [NetworkChuck](https://www.youtube.com/c/NetworkChuck)
- [TechWorldwithNana](https://www.youtube.com/c/TechWorldwithNana)

When you are not sure about what is out there in terms of technologies and resources, always consult with your local awesome list:

- [AcalephStorage/awesome-devops](https://github.com/AcalephStorage/awesome-devops)
- [awesome-soft/awesome-devops](https://github.com/awesome-soft/awesome-devops)
- [Lets-DevOps/awesome-learning](https://github.com/Lets-DevOps/awesome-learning)
- [AcalephStorage/awesome-devops](https://github.com/AcalephStorage/awesome-devops)
- [awesome-selfhosted/awesome-selfhosted](https://github.com/awesome-selfhosted/awesome-selfhosted)
- [juandecarrion/awesome-self-hosted](https://github.com/juandecarrion/awesome-self-hosted)
- [kahun/awesome-sysadmin](https://github.com/kahun/awesome-sysadmin)
- [epcim/awesome-sysadmin2](https://github.com/epcim/awesome-sysadmin2)
- [devops-roadma](https://github.com/raycad/devops-roadmap)

### Tools

In order to move forward, it is better to have a virtual machine running Ubuntu 22.04 (or latest stable) with the following tools (latest stable versions) installed:

- asdf
- git
- docker
- minikube
- terraform (via asdf)
- kubectl (via asdf)
- helm (via asdf)
- nodejs (via asdf)
- npm (via asdf)
- ansible (via asdf)
- jq
- curl
- wget

You can find the official documentations to see how to install and configure the tools.

### Services

To ease your way into the DevOps world, we will be using the following services:

- Register at [GitHub.com](https://github.com).
- Register at [GitLab.com](https://gitlab.com).
- Register at [Azure DevOps](https://azure.microsoft.com/en-us/pricing/details/devops/azure-devops-services/).
- Register at [Docker Hub](https://hub.docker.com).
- Register at [Oracle](https://youtu.be/NKc3k7xceT8) for a free VM.
- Register at [Cloudflare](https://www.cloudflare.com/) for managing DNS zones.
-

### Extra

- If you are a student (or have a student email), get the [GitHub Student Developer Pack](https://education.github.com/pack).

## Task 1: Starting apps

TODO

### Task 1.1 Docker

TODO

### Task 1.2 Docker-compose

TODO

### Task 1.3 Kubernetes

TODO

## Task 2: Pipelines

TODO

### Task 2.1 Jenkins

TODO

### Task 2.2 Gitlab

TODO

### Task 2.3 Github

TODO

## Task 3: Data Formats

TODO

### Task 3.1 JSON

TODO

### Task 3.2 YAML

TODO

### Task 3.3 TOML

TODO

### Task 3.4 XML

TODO

### Task 3.5 CSV

TODO

### Task 3.6 INI

TODO

## Task 4: Infrastructure as Code

TODO

### Task 4.1 Terraform

TODO

### Task 4.2 Ansible

TODO

### Task 4.3 Pulumi

TODO

### Task 4.4 Puppet

TODO

### Task 4.5 Chef

TODO

### Task 4.6 SaltStack

TODO

## Task 5: Cloud Providers

TODO

### Task 5.1 AWS

TODO

### Task 5.2 Azure

TODO

### Task 5.3 GCP

TODO

### Task 5.4 Oracle

TODO

### Task 5.5 Digital Ocean

TODO

### Task 5.6 Linode

TODO

## Questions

Try to answer the following questions with a few sentences:

- TODO

## Terms, buzzwords and more

In order to understand the DevOps (and IT) world, you need to know the following terms, try to copy this table in a markdown file and fill in some information about how you understand the term, if the term has any tools or technologies that you can use for example and if it is not a technology - some use cases:

| Terms, buzzword and more             | Explain in one sentance | Provide example tools, technologies and use cases |
| ------------------------------------ | ----------------------- | ------------------------------------------------- |
| devops pipelines                     | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| containerization                     | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| continuous integration               | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| continuous delivery                  | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| continuous deployment                | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| build tools                          | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| container fleet management           | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| version control system               | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| source control system                | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| container orchestration              | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| artifact repository                  | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| AWS EC2                              | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| GCP Compute Instance                 | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| DevSecOps                            | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| immutable infrastructure             | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| server clustering                    | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| server failover                      | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| on-premise                           | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| high availability                    | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| configuration management             | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| repository branches                  | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| application performance monitoring   | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| logs management                      | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| dynamic scaling servers              | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| infrastructure resilience            | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| UAT                                  | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| regression testing                   | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| development environment              | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| testing environment                  | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| environment provisioning             | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| staging environment                  | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| bastion server                       | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| bare-metal server                    | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| cloud computing                      | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| big data                             | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| IaaS                                 | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| PaaS                                 | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| SaaS                                 | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| I/O throughput                       | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| Mean Time to Recovery                | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| linux distribution                   | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| rolling update                       | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| test automation                      | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| technical debt                       | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| VPC peering                          | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| software development lifecycle       | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| microservices                        | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| monolithic application               | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| type 1 hypervisor                    | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| bootloader                           | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| API                                  | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| deployment frequency                 | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| percentage of failed deployments     | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| distributed vs decentralized systems | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| continuous monitoring                | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| serverless computing                 | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| RAID                                 | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| script shebang                       | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| data science                         | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| deep learning                        | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| FOSS/FLOSS software                  | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| Blue/Green deployment                | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| A/B Testing                          | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| Canary releases                      | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| Rolling releases                     | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| Infrastructure as Code               | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| Compliance as Code                   | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| Security as Code                     | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| Pre-commit hooks                     | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| SAST                                 | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| DAST                                 | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| cloud agnostic                       | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| idempotent resource                  | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| SDLC                                 | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| tainted resource                     | [YOUR ANSWER]           | [YOUR ANSWER]                                     |

An example of how to fill in data:

| Terms, buzzword and more | Explain in one sentence                                    | Provide example tools, technologies and use cases                                                           |
| ------------------------ | ---------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------- |
| devops pipelines         | Automated workflows that orchestrate software delivery.    | Tools: Jenkins, CircleCI, GitLab CI/CD. Use Cases: Continuous delivery, deployment automation.              |
| containerization         | Packaging applications along with their dependencies.      | Technologies: Docker, Kubernetes. Use Cases: Scalable and portable deployments, microservices architecture. |
| continuous integration   | Regularly integrating code changes to detect issues early. | Tools: Travis CI, Jenkins, GitLab CI/CD. Use Cases: Early bug detection, ensuring code quality.             |
