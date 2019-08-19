# Multi Tier Docker Application

[![Build Status](https://travis-ci.org/samirprakash/multi-tier-docker.svg?branch=master)](https://travis-ci.org/samirprakash/multi-tier-docker)

#### Architecture

![alt project architecture](./screenshots/multi-tier-docker-app-architecture.png)

#### Flow

![alt project flow](./screenshots/multi-tier-docker-app-flow.png)

#### Production Multi Container Setup

![alt multi container setup](./screenshots/multi-tier-production-setup.png)

#### Production ECS setup architecture

![alt ESC setup](./screenshots/multi-tier-aws-eb.png)

#### AWS Steps

- Create Elastic Beanstalk environment with multi docker support (EBS)
- AWS elastic cache for redis (EC)
- AWS Relational Database Service (RDS) for Postgres
- Check VPC
- Create Security Group connection EBS, RDS and EC
- Create RDS
- Create EC
- Create Security Group with default VPC abd set inbound rules
- Update Security Group in EBS, RDS and EC instances
- Add environment variables in EBS
