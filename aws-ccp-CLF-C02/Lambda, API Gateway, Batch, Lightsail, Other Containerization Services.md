**Docker**
- apps are packaged into *containers*
- docker daemon

**Serverless**
- devs don't manage servers; just deploy code/functions
- servers are fully managed by AWS

***

**ECS**
- launch docker containers in AWS (via EC2 - *provision by user*)
- AWS starts/stops containers

**Fargate**
- "serverless" launch docker containers in AWS (via EC2 - *provision by AWS*)

**ECR**
- private docker registry in AWS
- place to store docker images

***


**Lambda**
- functions (virtual) in the cloud
- run *on-demand*
- automated scaling
- *event-driven*: run/triggered by AWS when needed
- monitoring via CloudWatch
- pricing: based on *calls* and *duration*

**API Gateway**
- serverless APIs
- supports RESTful and WebSocket APIs
- expose Lambda functions as HTTP APIs

**Batch**
- run (containerized) batch jobs on AWS
- launch **EC2 instance** and **Spot instances**
- batch jobs: defined as **docker images** & **run on EC2**
- not serverless; fully managed by AWS

**Lightsail**
- simple alternative to existing compute resources e.g. EC2
- has high availability but no auto-scaling