**CloudFormation**
- infrastructure as code
- declarative way:
	- create *templates* to describe and model all AWS resources needed 
	- CloudFormation provisions and configures resources in the template

**CDK**
- define and model cloud infra using *preferred* programing language
- code will be compiled into CF template (JSON/YAML)

**Beanstalk**
- deploying and scaling web apps in AWS
- PaaS, developer-centric
- managed service: focus on app code instead of manually managing resources in AWS
- architecture models
- health monitoring - health agents
	- view metrics inside beanstalk
- 