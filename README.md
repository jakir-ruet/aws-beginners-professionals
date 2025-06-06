## More About Me – [Take a Look!](http://www.mjakaria.me) 

### Welcome to Cloud Computing (AWS)
#### This Course Consist three segments
- [AWS Certified Developer Associate - CLF-02](https://aws.amazon.com/certification/certified-developer-associate/)
- [AWS Certified Cloud Practitioner - DVA-02](https://aws.amazon.com/certification/certified-cloud-practitioner/)
- [AWS Certified DevOps Engineer Professional - DOP-C02](https://aws.amazon.com/certification/certified-devops-engineer-professional/)

### [AWS Certified Developer Associate - CLF-02](https://aws.amazon.com/certification/certified-developer-associate/)
#### Introduction
The AWS Certified Cloud Practitioner exam is designed for individuals who can demonstrate foundational knowledge of the AWS Cloud, independent of a specific job role. The exam validates a candidate’s ability to complete the following tasks: 
- Explain the value of the AWS Cloud. 
- Understand and explain the AWS shared responsibility model. 
- Understand security best practices. 
- Understand AWS Cloud costs, economics, and billing practices. 
- Describe and position the core AWS services, including compute, network, database, and storage services. 
- Identify AWS services for common use cases.

#### Target Candidate
The target candidate has up to 6 months of exposure to AWS Cloud design, implementation, and/or operations. This certification is ideal for candidates who are from non-IT backgrounds. These candidates might be in the early stages of pursuing an AWS Cloud career or might work with people in AWS Cloud roles. 

#### Recommended AWS Knowledge 
The target candidate should have AWS knowledge in the following areas: 
- AWS Cloud concepts 
- Security and compliance in the AWS Cloud 
- Core AWS services 
- Economics of the AWS Cloud

#### Not Need to Know (Job tasks that are out of scope for the target candidate)
The following list contains job tasks that the target candidate is not expected to be able to 
perform. This list is non-exhaustive. These tasks are out of scope for the exam: 
- Coding 
- Cloud architecture design 
- Troubleshooting 
- Implementation 
- Load and performance testing 
Refer to `Appendix A` for a list of technologies and concepts that might appear on the exam, a list of in-scope AWS services and features, and a list of out-of-scope AWS services and features.

#### Exam Content 
Response types `>` There are two types of questions on the exam: 
- `Multiple choice:` Has `one correct` response and three incorrect responses (distractors) 
- `Multiple response:` Has `two or more correct` responses out of five or more response 
options

#### Instructions
- Select one or more responses that `best complete` the statement or answer the question.
- Distractors, or incorrect answers, are response options that a candidate with incomplete knowledge or skill might choose. 
- Distractors are generally plausible responses that match the content area. 
- Unanswered questions are scored as `incorrect`; there is `no penalty` for guessing. 
- The exam includes `50` questions that affect your score.

#### Exam Score
| SL  | Title           | Marks                                        |
| --- | --------------- | -------------------------------------------- |
| 1   | Total Questions | 65 (50 Scored + 15 Un-scored)                |
| 2   | Passing Score   | 700/1000                                     |
| 3   | Scoring Model   | Compensatory (Pass Overall, Not per Section) |
| 4   | Validity        | 3 Years                                      |

The exam has the following content domains and weightings:
| Domain | Description                   | Weight |
| ------ | ----------------------------- | ------ |
| 1      | Cloud Concepts                | 24%    |
| 2      | Security and Compliance       | 30%    |
| 3      | Cloud Technology and Services | 34%    |
| 4      | Billing, Pricing, and Support | 12%    |

#### AWS CLI Configuration
- Control multiple AWS services from this command line.
- How to [Install?](https://docs.aws.amazon.com/cli/latest/userguide/getting-started-install.html)
- Let's me check `aws --version`
- If its okay then we will see `aws-cli/2.15.4 Python/3.11.6 Darwin/23.2.0 exe/x86_64 prompt/off`
- Configuration using security credential
 - Go to AWS Management Console > Services > IAM
 - Select the IAM User Name: Your User Name [_**NB**_: You must use IAM's Information only not Root User]
 - Click on `Security credentials`
 - Click on `Create access key`
 - Copy Access ID & Secret access key
 - Go to your Terminal and implement as below format
 - `aws configure`
 - AWS Access Key ID [None]: Put your ID here and press Enter.
 - AWS Secret Access Key [None]: Put your secret key here and press Enter
 - Default region name [None]: us-east-1
 - Default output format [None]: json
- Let's me check whether the configuration is done.
 - `aws ec2 describe-vpcs`
 - If it is done then we will see the details of the default vpc.

#### Domain 1: Cloud Concepts
##### Cloud Computing
Cloud computing is the on-demand delivery of compute power, database, storage, applications, and other IT resources through a cloud services platform via the internet with pay-as-you-go pricing.

##### [Types of Cloud Computing Deployment Models](https://aws.amazon.com/types-of-cloud-computing/)
- [Private Cloud](https://aws.amazon.com/what-is/private-cloud/#:~:text=A%20private%20cloud%20is%20a,the%20control%20of%20one%20organization.)
  - This service used by a single organization, not exposed to public.
  - Complete self control
  - Secure for sensitive applications.
  - Fulfill specified requirements.
  - For example [RackSpace](https://www.rackspace.com), [Hewlett Packard Enterprise (HPE)](https://www.hpe.com/emea_europe/en/home.html) and so on.
- Public Cloud
  - Cloud resources owned and operated by a third- party cloud service provider delivered over the Internet.
  - [Six Advantages](https://docs.aws.amazon.com/whitepapers/latest/aws-overview/six-advantages-of-cloud-computing.html) of Cloud Computing.
    - Trade fixed expense (Capital Expense - ***CapEx***) for variable expense (Operational Expense - ***OpEx***).
      - Pay on demand: Don't own hardware.
      - Reduce Total Cost of Ownership (TCO) & Operational Expense (OpEx).
    - Benefit from massive economies of scale
      - Prices are reduced as AWS is more efficient due to large scale
    - Stop guessing capacity
      - Scale based on actual measured usage
    - Increase speed and agility
    - Stop spending money running and maintaining data centers
    - Go global in minutes
  - For example AWS, Google Cloud Platform (GCP) & Microsoft Azure.
- [Hybrid Cloud](https://aws.amazon.com/hybrid/)
  - Keep some servers on premises and extend some capabilities to the Cloud
  - Control over sensitive assets in your private infrastructure
  - Flexibility and cost- effectiveness of the public cloud
  - For example, On-premises with Public cloud.

##### The Five Characteristics of Cloud Computing
1. On-demand self service:
   Users can provision resources and use them without human interaction from the service provider
2. Broad network access:
   Resources available over the network, and can be accessed by diverse client platforms
3. Multi-tenancy and resource pooling:
   Multiple customers can share the same infrastructure and applications with security and privacy.
   Multiple customers are serviced from the same physical resources
4. Rapid elasticity and scalability:
   Automatically and quickly acquire and dispose resources when needed
   Quickly and easily scale based on demand
5. Measured service:
   Usage is measured, users pay correctly for what they have used

##### Problems solved by the Cloud
- Flexibility: change resource types when needed
- Cost-Effectiveness: pay as you go, for what you use
- Scalability: accommodate larger loads by making hardware stronger or adding additional nodes
- Elasticity: ability to scale out and scale-in when needed
- High-availability and fault-tolerance: build across data centers
- Agility: rapidly develop, test and launch software applications

##### [Types of Cloud Computing Model](https://aws.amazon.com/types-of-cloud-computing/)
- Infrastructure as a Service (IaaS)
  - Provide building blocks for cloud IT
  - Provides networking, computers, data storage space
  - Highest level of flexibility
  - Easy parallel with traditional on-premises IT
  - For example
    - Amazon EC2 (on AWS)
    - GCP, Azure, Rackspace, Digital Ocean, Linode
- Platform as a Service (PaaS)
  - Removes the need for your organization to manage the underlying infrastructure
  - Focus on the deployment and management of your applications
  - For example
    - Elastic Beanstalk (on AWS)
    - Heroku, Google App Engine (GCP), Windows Azure (Microsoft)
- Software as a Service (SaaS)
  - Completed product that is run and managed by the service provider
  - For example
    - Many AWS services (ex: Rekognition for Machine Learning)
    - Google Apps (Gmail), Dropbox, Zoom
  
##### Cloud Computing Model
![Cloud Computing Model](/img/cloud-computing-model.png)

##### Highly Available and Scalable Resources
High availability means your application or service remains **accessible and operational** even when one or more components fail. Key Features:
- Redundancy
- Failover mechanisms
- Health checks and monitoring

##### AWS Services Supporting High Availability:
| Service                         | High Availability Feature                         |
| ------------------------------- | ------------------------------------------------- |
| **Amazon EC2**                  | Use Auto Scaling + Load Balancer across AZs       |
| **Elastic Load Balancer (ELB)** | Distributes traffic across multiple instances/AZs |
| **Amazon RDS (Multi-AZ)**       | Automatic failover to standby instance            |
| **Amazon S3**                   | Stores data across multiple AZs                   |
| **Route 53**                    | DNS-level failover and health checks              |
| **Amazon DynamoDB**             | Automatically replicates data across multiple AZs |

##### Scalability, Elasticity & Agility
Scalability, Elasticity, and Agility are core principles that underpin the cloud computing model, enabling businesses to meet fluctuating demand, optimize costs, and innovate faster. These are cloud concepts that help applications handle varying loads efficiently — but they are `not the same` thing.

###### Scalability
The ability of a system to increase or decrease its capacity (usually compute, storage, or throughput) based on workload. Types of Scalability:
- Vertical Scaling (Scaling Up/Down)
  - Add more power (CPU/RAM) to an existing instance.
  - Example: Change an EC2 instance from `t2.micro` to `t3.large`.
- Horizontal Scaling (Scaling Out/In)
  - Add or remove multiple instances to distribute the load.
  - Example: Add more EC2 instances to a load balancer group.

- AWS Services That Support Scalability:
  - EC2 Auto Scaling
  - Elastic Load Balancing
  - Amazon RDS (Read Replicas for horizontal read scalability)
  - Amazon DynamoDB (auto scaling read/write capacity)

###### Elasticity
The ability of the system to automatically adjust capacity to maintain performance as demand changes in real-time. Think of it as automated and reactive scalability.
- AWS Services That Provide Elasticity:
  - EC2 Auto Scaling Groups (ASG): Automatically increase/decrease EC2 instances based on demand.
  - AWS Lambda: Automatically scales based on the number of incoming requests.
  - Amazon Aurora Serverless: Automatically adjusts database capacity.

 ###### Agility
**Agility** in cloud computing refers to the ability to **quickly adapt** to changes in demand or business needs by leveraging scalable, flexible, and automated cloud resources. In AWS, agility allows businesses to deploy, scale, and modify their infrastructure with minimal time and effort.

###### Key Features of Agility
- `Rapid Deployment:` Launch services, applications, and infrastructure quickly without needing to wait for physical hardware or lengthy configuration processes.
- `Flexibility and Adaptability:` Change infrastructure configurations in real-time to meet new demands or operational requirements.
- `Cost Efficiency:` Only pay for what you use, enabling teams to experiment with new ideas without worrying about upfront costs.
- `Automation:` Automate resource management and application deployment to save time and reduce human error.

###### Agility vs Traditional IT
| Aspect           | Traditional IT                         | Cloud Agility (AWS)                   |
| ---------------- | -------------------------------------- | ------------------------------------- |
| Deployment Speed | Slow, manual provisioning of hardware  | Fast, automated resource provisioning |
| Scalability      | Limited by hardware, requires planning | Auto-scaling based on demand          |
| Flexibility      | Difficult to change configurations     | Easily adaptable to meet new needs    |
| Cost Efficiency  | High upfront costs                     | Pay-as-you-go, no upfront investment  |

###### Key Differences Between Scalability and Elasticity
| Feature        | Scalability                              | Elasticity                                 |
| -------------- | ---------------------------------------- | ------------------------------------------ |
| Focus          | Capacity expansion                       | Real-time responsiveness                   |
| Trigger        | Manual or rule-based                     | Automated and reactive                     |
| Example        | Add more EC2 instances with Auto Scaling | Lambda scales automatically with requests  |
| Resource Usage | Grows with load (needs configuration)    | Expands/contracts on demand without effort |

##### Architecting for the Cloud
The design principles of the AWS Cloud, primarily guided by the `AWS Well-Architected Framework`. These principles help you build secure, high-performing, resilient, and efficient infrastructure on the cloud.

###### [AWS Well-Architected Framework](https://docs.aws.amazon.com/wellarchitected/latest/framework/welcome.html)
The AWS Well-Architected Framework helps you understand the `pros` and `cons` of decisions you make while building systems on AWS. By using the Framework you will learn architectural best practices for designing and operating `reliable`, `secure`, `efficient`, `cost-effective`, and `sustainable` systems in the cloud.

###### AWS Well-Architected and the [Six Pillars](https://aws.amazon.com/architecture/well-architected/?ref=wellarchitected-wp&wa-lens-whitepapers.sort-by=item.additionalFields.sortDate&wa-lens-whitepapers.sort-order=desc&wa-guidance-whitepapers.sort-by=item.additionalFields.sortDate&wa-guidance-whitepapers.sort-order=desc)
- Operational Excellence Pillar
- Security Pillar
- Reliability Pillar
- Performance Efficiency Pillar
- Cost Optimization Pillar
- Sustainability Pillar

###### The Six Pillars of the AWS Well-Architected Framework
1. `Operational Excellence:` Run and monitor systems to deliver business value and continually improve processes. Key Design Principles:
- Perform operations as code
- Annotate documentation
- Make frequent, small, reversible changes
- Refine operations procedures
- Anticipate failure
- Learn from all operational events and failures

2. `Security:` Protect information, systems, and assets while delivering business value. Key Design Principles:
- Implement a strong identity foundation
- Enable traceability
- Apply security at all layers
- Automate security best practices
- Protect data in transit and at rest
- Keep people away from data
- Prepare for security events

3. `Reliability:` Ensure a workload performs its intended function correctly and consistently. Key Design Principles:
- Test recovery procedures
- Automatically recover from failure
- Scale horizontally to increase availability
- Stop guessing capacity
- Manage change in automation

4. `Performance Efficiency:` Use computing resources efficiently to meet system requirements and maintain efficiency as demand changes. Key Design Principles:
- Democratize advanced technologies
- Go global in minutes
- Use serverless architectures
- Experiment more often
- Consider mechanical sympathy (use the right tool for the job)

5. `Cost Optimization:` Avoid unnecessary costs and understand where money is being spent. Key Design Principles:
- Adopt a consumption model
- Measure overall efficiency
- Stop spending money on undifferentiated heavy lifting
- Analyze and attribute expenditures
- Use managed and serverless services to reduce costs

6. `Sustainability (Introduced in 2021):` Minimize environmental impact of running cloud workloads. Key Design Principles:
- Understand your impact
- Establish sustainability goals
- Maximize utilization
- Reduce downstream impact (e.g., client-side optimization)
- Continually innovate for sustainability

###### Summary of Pillar
| **Pillar**             | **Focus Area**                                        |
| ---------------------- | ----------------------------------------------------- |
| Operational Excellence | Monitoring, incident response, continuous improvement |
| Security               | Identity, access, detection, data protection          |
| Reliability            | Fault tolerance, recovery, scaling                    |
| Performance Efficiency | Optimal resource selection and usage                  |
| Cost Optimization      | Spend control, budgeting, resource management         |
| Sustainability         | Environmental impact and energy efficiency            |

###### Multi-Tenant Architectures
Multi-tenancy in the cloud refers to an architecture where a single instance of a cloud service or application serves multiple customers (tenants). Each tenant's data, configurations, and operations are isolated, but they share the same underlying infrastructure. This approach is commonly used in cloud computing to reduce costs and maximize resource utilization while maintaining data separation and security between tenants. Three types of Multi-Tenancy:
1. Silo Model
2. Bridge Model
3. Pool Model

![Multi-Tenant Architectures](/img/multi-tenant-architectures.png)

**Comparison Table: Silo Model vs. Bridge Model vs. Pool Model**
![Multi-Tenant Architectures](/img/comparison-silo-bridge-pool.png)

##### Management and Governance
###### [AWS Control Tower](https://docs.aws.amazon.com/organizations/latest/userguide/services-that-can-integrate-CTower.html)
AWS Control Tower offers a straightforward way to set up and govern an AWS multi-account environment, following prescriptive best practices. AWS Control Tower orchestration extends the capabilities of AWS Organizations. AWS Control Tower applies preventive and detective controls (guardrails) to help keep your organizations and accounts from divergence from best practices (drift).
**Features for AWS Control Tower**
- Set up multi-account environment quickly
- Automation and built-in governance
- Preconfigured Controls
- Integrate third-party software at scale

###### [AWS Organizations](https://docs.aws.amazon.com/organizations/latest/userguide/orgs_introduction.html)
AWS Organizations is a service from Amazon Web Services that lets you centrally manage and govern multiple AWS accounts. It’s especially useful for businesses that want to create separate AWS accounts for different departments, projects, or teams while still keeping control from a central location.

**Features for AWS Organizations**
- Manage your AWS accounts
- Define and manage your organization
- Secure and monitor your accounts
- Share resources across accounts
- Audit your environment for compliance
- Centrally manage billing and costs

**Architechure**
![Architechure](/img/organization-control-tower.png)

###### Landing Zone
A Landing Zone within AWS Control Tower is a securely architected multi-account AWS environment where you enforce certain compliance and security best practices. Basically, it is the container that holds all of your organization units, accounts, users, and other resources that you want to be subject to a particular set of compliance restrictions. It automates the setup using predefined blueprints for identity management, federated access, and account structures, which include centralized logging and cross-account security audits.

###### Service Control Policies
In AWS Organizations used to manage and enforce governance rules across multiple AWS accounts. SCPs enable you to define the maximum available permissions for accounts within your organization, providing a central way to control which AWS services and actions can be accessed by users and roles in those accounts.

**Comparison between AWS Organization and AWS Control Tower**
| Feature              | **AWS Organizations**                                        | **AWS Control Tower**                                               |
| -------------------- | ------------------------------------------------------------ | ------------------------------------------------------------------- |
| **Purpose**          | Manually manage multiple AWS accounts, billing, and policies | Automate the setup of a secure, compliant multi-account environment |
| **Setup Complexity** | Low-level, manual setup required                             | High-level, guided setup with automation                            |
| **Account Creation** | Manually create accounts via CLI/API or console              | Automates account creation via **Account Factory**                  |
| **Governance**       | Uses **Service Control Policies (SCPs)**                     | Uses SCPs, plus **Guardrails** (prebuilt SCPs and AWS Config rules) |
| **Landing Zone**     | You build your own                                           | Prebuilt landing zone architecture (AWS best practices)             |
| **UI**               | No dedicated UI – uses AWS Console/CLI                       | Dedicated dashboard for governance and account management           |
| **Ideal For**        | Advanced users, custom setups                                | Medium to large organizations looking for fast, standardized setup  |

###### [AWS Systems Manager](https://docs.aws.amazon.com/organizations/latest/userguide/services-that-can-integrate-ssm.html)
AWS Systems Manager is a collection of capabilities that enable visibility and control of your AWS resources. The following Systems Manager capabilities work with Organizations across all of the AWS accounts in your organization:
###### [AWS Service Catalog](https://docs.aws.amazon.com/whitepapers/latest/introduction-devops-aws/aws-service-catalog.html)
AWS Service Catalog enables organizations to create and manage catalogs of IT services that are approved for AWS. These IT services can include everything from virtual machine images, servers, software, databases, and more to complete multi-tier application architectures.
###### [AWS Config](https://docs.aws.amazon.com/controltower/latest/userguide/config.html)
AWS Config provides a detailed view of the resources associated with your AWS account, including how they are configured, how they are related to one another, and how the configurations and their relationships have changed over time.
###### [AWS Trusted Advisor](https://docs.aws.amazon.com/awssupport/latest/user/trusted-advisor.html)
Trusted Advisor draws upon best practices learned from serving hundreds of thousands of AWS customers. Trusted Advisor inspects your AWS environment, and then makes recommendations when opportunities exist to save money, improve system availability and performance, or help close security gaps.

##### Deployment, [Migration & Transfer](https://docs.aws.amazon.com/whitepapers/latest/aws-overview/migration-services.html) to the AWS Cloud.
In AWS (Amazon Web Services), deployment, migration, and transfer are key concepts related to moving applications, data, or infrastructure into or within the cloud. Here's a breakdown of each:

###### [Deployment](https://docs.aws.amazon.com/whitepapers/latest/introduction-devops-aws/deployment-strategies.html)
Deployment strategies define how you want to deliver your software. Organizations follow different deployment strategies based on their business model. Some choose to deliver software that is fully tested, and others might want their users to provide feedback and let their users evaluate under development features (such as Beta releases). The following section discusses various deployment strategies.
- Deployment Models:
  - [In-place deployments](https://docs.aws.amazon.com/whitepapers/latest/overview-deployment-options/in-place-deployments.html)
    An in-place deployment is a deployment strategy that updates the application version without replacing any infrastructure components. In an in-place deployment, the previous version of the application on each compute resource is stopped, the latest application is installed, and the new version of the application is started and validated.
  - [Blue/Green Deployment](https://docs.aws.amazon.com/whitepapers/latest/blue-green-deployments/welcome.html)
    The blue/green deployment technique enables you to release applications by shifting traffic between two identical environments that are running different versions of the application. Blue/green deployments can mitigate common risks associated with deploying software, such as downtime and rollback capability.
  - [Canary Deployment](https://docs.aws.amazon.com/whitepapers/latest/overview-deployment-options/canary-deployments.html)
    Canary deployments are a type of blue/green deployment strategy that is more risk-averse. This strategy involves a phased approach in which traffic is shifted to a new version of the application in two increments. The first increment is a small percentage of the traffic, which is referred to as the canary group.
  - [Linear deployment](https://docs.aws.amazon.com/whitepapers/latest/introduction-devops-aws/deployment-strategies.html)
    Linear deployment means traffic is shifted in equal increments with an equal number of minutes between each increment. You can choose from predefined linear options that specify the percentage of traffic shifted in each increment and the number of minutes between each increment.
  - [All-at-once deployment](https://docs.aws.amazon.com/whitepapers/latest/introduction-devops-aws/deployment-strategies.html)
    All-at-once deployment means all traffic is shifted from the original environment to the replacement environment all at once.
  - [Rolling Deployment](https://docs.aws.amazon.com/whitepapers/latest/overview-deployment-options/rolling-deployments.html)
    A rolling deployment is a deployment strategy that slowly replaces previous versions of an application with new versions of an application by completely replacing the infrastructure on which the application is running.
  - [Immutable Deployment](https://docs.aws.amazon.com/elasticbeanstalk/latest/dg/environmentmgmt-updates-immutable.html)
    Immutable environment updates are an alternative to rolling updates. Immutable environment updates ensure that configuration changes that require replacing instances are applied efficiently and safely. If an immutable environment update fails, the rollback process requires only terminating an Auto Scaling group.

Deployment Matrix
| Deployment Strategy | Amazon ECS | AWS Lambda | Amazon EC2/on-premises |
| ------------------- | ---------- | ---------- | ---------------------- |
| In-place            | ✓          | ✓          | ✓                      |
| Blue/green          | ✓          | ✓          | ✓*                     |
| Canary              | ✓          | ✓          | X                      |
| Linear              | ✓          | ✓          | X                      |
| All-at-once         | ✓          | ✓          | X                      |

###### Migration
**Prerequisite of Migration**
| Phase       | Key Activities                                                            |
| ----------- | ------------------------------------------------------------------------- |
| Preparation | Current Architecture, assess environment, choose strategy                 |
| Planning    | Estimate cost, design architecture, monolithic to microservice            |
| Migrate     | Use AWS tools (MGN, DMS), test, validate, backup, cutover                 |
| Monitor     | Track performance with CloudWatch, CloudTrail, X-Ray, set alerts          |
| Optimize    | Right-size resources, cost optimization, enhance security, modernize apps |

**Migration Strategies (7 R’s)**
| Strategy   | Description                                                              |
| ---------- | ------------------------------------------------------------------------ |
| Refactor   | Redesign application for cloud-native architecture (e.g., microservices) |
| Replatform | "Lift, tinker, and shift" – make minimal changes (e.g., move DB to RDS)  |
| Repurchase | Replace with SaaS solutions (e.g., move to a cloud-based CRM)            |
| Rehost     | "Lift and shift" – move applications to AWS without changes              |
| Relocate   | Move without modification "Lift and shift"                               |
| Retain     | Keep some apps on-premises (temporarily or permanently)                  |
| Retire     | Decommission outdated or unused applications                             |

AWS offers a comprehensive suite of tools and services to facilitate cloud migration, including automated processes and specialized expertise. 
- [AWS Migration Evaluator](https://aws.amazon.com/migration-evaluator/?p=ft&c=mg&z=3)
  Helps build a business case for cloud migration by analyzing on-premises infrastructure usage and costs. What it does:
  - Collects data from on-prem environments (agentless).
  - Provides cost projections for running workloads on AWS.
  - Helps identify underutilized resources and potential savings.
  - Best for: Pre-migration cost analysis and planning.
- [AWS Application Discovery Service](https://aws.amazon.com/application-discovery/?p=ft&c=mg&z=3)
  Discovers on-premises servers to gather information about their configuration, usage, and behavior What it does:
  - Can use agents or agentless discovery.
  - Collects data like CPU, memory, network usage, and running processes.
  - Helps map application dependencies.
  - Best for: Understanding your current environment before migration.
- [AWS Migration Hub](https://aws.amazon.com/migration-hub/?p=ft&c=mg&z=3)
  Centralized tracking and monitoring of migration progress across AWS services. What it does:
  - Provides a single pane of glass for tracking application migrations.
  - Integrates with other migration tools (like Application Migration Service and DMS).
  - Can group resources by application for easier tracking.
  - Best for: Managing and coordinating large-scale migrations.
- [AWS Application Migration Service - MGN](https://aws.amazon.com/application-discovery/?p=ft&c=mg&z=3)
  Simplifies and automates the lift-and-shift (rehost) of physical, virtual, or cloud servers to AWS. What it does:
  - Real-time replication of source servers.
  - Minimal downtime cutover.
  - Automated post-launch modernization (e.g., instance type changes).
  - Best for: Rehosting existing workloads with minimal changes.
- [AWS Database Migration Service - DMS](https://aws.amazon.com/migration-hub/?p=ft&c=mg&z=3)
  Migrates databases to AWS quickly and securely with minimal downtime. What it does:
  - Supports homogenous (e.g., Oracle to Oracle) and heterogeneous (e.g., SQL Server to Aurora) migrations.
  - Can handle on-going replication for hybrid scenarios.
  - Best for: Database-specific migrations, both one-time and continuous replication.
- [AWS Migration Acceleration Program (MAP)](https://aws.amazon.com/migration-acceleration-program/)
  The AWS Migration Acceleration Program (MAP) is a structured framework provided by Amazon Web Services to help organizations accelerate their cloud migration journey. It's especially useful for enterprises planning large-scale migrations from on-premises or other cloud environments to AWS.
- [Cloud Migration Factory (CMF)](https://aws.amazon.com/solutions/implementations/cloud-migration-factory-on-aws/)
  A Cloud Migration Factory is a centralized migration model that industrializes the migration process, breaking it into repeatable units. Think of it like an assembly line for cloud migration—each step is standardized to improve speed, reduce errors, and ensure consistency.

![Here's a comparison table that highlights the key differences between the AWS migration-related services you mentioned:](/img/cloud-migration.png)

###### Data Transfer
AWS Data Transfer Services, which help you move data to, from, and within the AWS Cloud — whether online, offline, in real-time, or bulk.
- [AWS Snow Family](https://aws.amazon.com/snowball/) > `Snowcone / Snowball / Snowmobile`
  The AWS Snow Family is a collection of physical devices that help you move data into and out of AWS, especially when dealing with large-scale data or limited internet connectivity.
  - Use case: Physical data transfer.
  - Snowcone: Up to 8 TB.
  - Snowball: ~50–80 TB per device.
  - Snowmobile: For exabyte-scale transfers.
  - Best for: Large offline transfers or when bandwidth is limited.
- [AWS Transfer Family](https://aws.amazon.com/aws-transfer-family/?c=mt&sec=srv)
  The AWS Transfer Family is all about enabling secure file transfers to and from AWS, using familiar and traditional protocols like SFTP, FTPS, and FTP — but fully managed and integrated with AWS services.
  - Use case: Managed SFTP, FTPS, FTP servers.
  - Supports: S3, EFS as backends.
  - Best for: Legacy systems integration via file transfer protocols.
- [AWS Mainframe Modernization Service](https://aws.amazon.com/mainframe-modernization/?c=mt&sec=srv)
  AWS Mainframe Modernization service is a unique platform that allows you to migrate and modernize your on-premises mainframe applications.
- [AWS DataSync](https://aws.amazon.com/datasync/?c=mt&sec=srv) > `Online`
  AWS DataSync is a fully managed data transfer service that simplifies, automates, and accelerates like `1.` On-prem → AWS (like S3, EFS, FSx), `2.` AWS → On-prem & `3.` Between AWS services/regions.
  - Use case: Automated data transfer between on-prem storage and AWS.
  - Supports: NFS, SMB, Amazon S3, EFS, FSx.
  - Pros: Fast, secure, can run on schedule.
  - Best for: Recurring or large-scale data migration.
- Developer-Friendly Tools
  - AWS CLI & SDKs
  - [Amazon Kinesis Data Firehose](https://aws.amazon.com/firehose/)
    It's a fully managed service provided by AWS that allows you to easily capture, transform, and load streaming data into various destinations like Amazon S3, Amazon Redshift, Amazon Elasticsearch Service (Amazon OpenSearch Service), and more. It’s part of the Kinesis family of services, which are designed to handle real-time data streaming.
    - Use case: Real-time streaming data to AWS services (S3, Redshift, etc.).
    - Best for: Logs, metrics, real-time data pipelines.
  - [AWS Glue](https://aws.amazon.com/glue/)
    It's a serverless data integration service provided by Amazon Web Services. It helps you discover, prepare, move, and transform data for analytics, machine learning, and application development.
    - Use case: ETL (Extract, Transform, Load).
    - Supports: S3, RDS, Redshift, JDBC, and more.
    - Best for: Data lakes, data warehouse migrations.

![Here's a comparison table that highlights the key differences between the AWS Data Transfer-related services you mentioned:](/img/data-transfer.png)

##### [Cloud Adoption Framework (CAF):](https://aws.amazon.com/cloud-adoption-framework/)
It's leverages AWS experience and best practices to help you digitally transform and accelerate your business outcomes through innovative use of AWS. AWS CAF identifies specific organizational capabilities that underpin successful cloud transformations. These capabilities provide best practice guidance that helps you improve your cloud readiness. AWS CAF groups its capabilities in `six` perspectives: 
- Business, 
- People, 
- Governance, 
- Platform, 
- Security, and 
- Operations. 

###### How AWS CAF brings tangible benefits across different business goals:
1. Reduced Business Risk
   - Resilience & Continuity: By leveraging AWS's global infrastructure and built-in redundancy, organizations reduce the risk of outages and data loss.
   - Security Best Practices: The CAF emphasizes a strong security posture, helping identify and address vulnerabilities early in the cloud journey.
   - Regulatory Compliance: The framework guides compliance with industry and government regulations, reducing legal and financial risk.
2. Improved ESG (Environmental, Social, and Governance) Performance
   - Environmental: Migrating to AWS can reduce carbon emissions as AWS operates on renewable energy and efficiently manages data centers.
   - Social: Upskilling employees for cloud roles creates new career opportunities and enhances workforce development.
   - Governance: CAF promotes transparency, accountability, and strong governance models that align with ethical and compliance standards.
3. Increased Revenue
   - Faster Time-to-Market: With cloud agility, businesses can innovate faster, roll out products more quickly, and capitalize on market opportunities.
   - Customer Experience: Enhanced digital services lead to better customer satisfaction and retention.
   - Global Reach: Access to AWS's global infrastructure supports expansion into new regions and customer bases.
4. Increased Operational Efficiency
   - Automation & Optimization: CAF encourages automating routine tasks and optimizing cloud resources, reducing manual work and costs.
   - Scalability & Flexibility: Resources can be scaled up or down based on demand, avoiding overprovisioning
   - Process Improvements: The framework helps streamline operations through best practices, monitoring, and continuous improvement models.

##### IaC, Provisioning - CloudFormation, Terraform
- Faster deployments: Automate the creation and management of infrastructure.
- Consistency: Reduce errors by using templates.
- Scalability: Easily replicate environments.
- Better management: Track changes with version control.
- Example: AWS CloudFormation lets you define your entire infrastructure in code (Infrastructure as Code, or IaC).

#### [02 Domain - Security and Compliance](https://aws.amazon.com/products/security/)
In AWS, **security** is a shared responsibility between AWS and the customer. To help customers fulfill their responsibilities, AWS provides **security services, documentation, and tools**.

##### Overview
- Identity and access management
- Detection and response
- Data protection
- Compliance
- Network and application protection

##### Key Security Components - AWS Security, Identity, & Compliance services
- Identity and Access Management
  1. AWS Identity and Access Management (IAM) - Securely manage identities and access to AWS services and resources.
  2. AWS IAM Identity Center - Centrally manage workforce access to multiple AWS accounts and applications.
  3. Amazon Cognito - Implement secure, frictionless customer identity and access management that scales.
  4. Amazon Verified Permissions - Manage fine-grained permissions and authorization within custom applications.
  5. AWS Directory Service - Gain efficiency with a fully managed Microsoft Active Directory service.
  6. AWS Resource Access Manager - Simply and securely share your AWS resources across multiple accounts.
  7. AWS Organizations - Centrally manage your environment as you scale your AWS resources.

- Detection and Response
  1. Amazon GuardDuty - Protect AWS accounts with intelligent threat detection.
  2. Amazon Inspector - Automated and continual vulnerability management at scale.
  3. AWS Security Hub - Automate AWS security checks and centralize security alerts.
  4. Amazon Security Lake - Automatically centralize your security data in a few steps.
  5. Amazon Detective - Analyze and visualize security data to investigate potential security issues.
  6. AWS Security Incident Response - Prepare for, respond to, and recover from security events
  7. AWS Config - Assess, audit, and evaluate configurations of your resources.
  8. Amazon CloudWatch - Observe and monitor resources and applications on AWS, on premises, and on other clouds.
  9. AWS CloudTrail - Track user activity and API usage.
  10. AWS IoT Device Defender - Security management across your IoT devices and fleets.
  11. AWS Elastic Disaster Recovery - Scalable, cost-effective application recovery to AWS.

- Network and Application Protection
  1. AWS Firewall Manager - Centrally configure and manage firewall rules across your accounts.
  2. AWS Network Firewall - Deploy network firewall security across your VPCs.
  3. AWS Shield - Maximize application availability and responsiveness with managed DDoS protection.
  4. AWS Verified Access - Provide secure access to corporate applications without a VPN.
  5. AWS Web Application Firewall (WAF) - Protect your web applications from common exploits.
  6. Amazon Route 53 Resolver DNS Firewall - Filter and control outbound DNS traffic for your VPCs.

- Data Protection
  1. Amazon Macie - Discover and protect your sensitive data at scale.
  2. AWS Key Management Service (AWS KMS) - Create and control keys to encrypt or digitally sign your data.
  3. AWS CloudHSM - Manage single-tenant hardware security modules (HSMs) on AWS.
  4. AWS Certificate Manager - Provision and manage SSL/TLS certificates with AWS services and connected resources.
  5. AWS Payment Cryptography - Simplify cryptography operations in your cloud-hosted payment applications.
  6. AWS Private Certificate Authority - Create private certificates to identify resources and protect data.
  7. AWS Secrets Manager - Centrally manage the lifecycle of secrets.

- Compliance
  1. AWS Artifact - No cost, self-service portal for on-demand access to AWS’ compliance reports.
  2. AWS Audit Manager - Continually audit your AWS usage to simplify risk and compliance assessment.

######  [Identity & Access Management (IAM)](https://docs.aws.amazon.com/IAM/latest/UserGuide/introduction.html)
AWS Identity and Access Management (IAM) is a web service that helps you securely control access to AWS resources. With IAM, you can centrally manage permissions that control which AWS resources users can access. Features of Identity and Access Management;
- It is global service
- Root account created by default, shouldn’t be used or shared
- Users are people within your organization, & can be grouped
- Groups only contain users, not other groups
- Users don’t have to belong to a group, and user can belong to multiple groups
- For an Example of group as follows
![iam-user](/img/iam-user.png)

###### Why use group
- The policies define the permission to the users.
- Users or Groups can be assigned JSON documents called policies
- These policies define the permissions of the users
- In AWS you apply the least privilege principle: don’t give more permissions than a user needs
- [Policies Structure](https://docs.aws.amazon.com/IAM/latest/UserGuide/access_policies.html)

###### [Policies Structure](https://docs.aws.amazon.com/IAM/latest/UserGuide/intro-structure.html)
***Principal:***
A principal is a human user or workload that can make a request for an action or operation on an AWS resource. After authentication, the principal can be granted either permanent or temporary credentials to make requests to AWS, depending on the principal type. IAM users and root user are granted permanent credentials, while roles are granted temporary credentials. As a best practice, we recommend that you require human users and workloads to access AWS resources using temporary credentials.
```JSON
{
  "Version": "2024-01-30",              // policy language version, always include
  "Id": "Account-Permission"            // an identifier for the policy (optional)
  "Statement": [                        // one/more individual statements (required)
    {
      "Sid": "FirstStatement",          // an identifier for the statement (optional)
      "Effect": "Allow",                // whether the statement allows/denies access (Allow, Deny)
      "Action": ["iam:ChangePassword"], // list of actions this policy allows/denies
      "Resource": "*"                   // list of resources to which the actions applied to
    },
    {
      "Sid": "SecondStatement",
      "Effect": "Allow",
      "Action": [
        "s3:List*",
        "s3:Get*"
      ],
      "Resource": [
        "arn:aws:s3:::confidential-data",
        "arn:aws:s3:::confidential-data/*"
      ],
      "Condition": {"Bool": {"aws:MultiFactorAuthPresent": "true"}} // conditions for when this policies in effect  (optional)
    }
  ]
}
```

##### Create IAM user in Hands on Class.
- Go the IAM section & press 'Create User'.
- Give the user name (JakirIam) as you like.
- Select the user type
  - Specify a user in Identity Center (Recommended)
  - I want to create an IAM user (selected)
  - Give the password as you like
- Press Next
- Create user group including define the permissions.
- Give the tag name (optional)
- Download credential csv file
- IAM user created.
- Create Access keys (Access & Secret Access key)

##### IAM Roles for Services
Some AWS service will need to perform actions on your behalf
 - To do so, we will assign permissions to AWS services with IAM Roles
 - Common roles: 
 - EC2 Instance Roles
   - Lambda Function Roles
   - Roles for CloudFormation

##### IAM Security Tools
- IAM Credentials Report (account-level)
  A report that lists all your account's users and the status of their various credentials
- IAM Access Advisor (user-level)
  - Access advisor shows the service permissions granted to a user and when those services were last accessed.
  - You can use this information to revise your policies.

##### Shared Responsibility Model of IAM
| AWS (Provider)                           | User                                                     |
| :--------------------------------------- | :------------------------------------------------------- |
| Infrastructure (global network security) | Users, Groups, Roles, Policies management and monitoring |
| Configuration and vulnerability analysis | Enable MFA on all accounts                               |
| Compliance validation                    | Rotate all your keys often                               |
| -                                        | Use IAM tools to apply appropriate permissions           |
| -                                        | Analyze access patterns & review permissions             |

##### [Shared Responsibility Model](https://aws.amazon.com/compliance/shared-responsibility-model/)
Security and Compliance is a shared responsibility between AWS and the customer. This shared model can help relieve the customer’s operational burden as AWS operates, manages and controls the components from the host operating system and virtualization layer down to the physical security of the facilities in which the service operates. The customer assumes responsibility and management of the guest operating system (including updates and security patches), other associated application software as well as the configuration of the AWS provided security group firewall. 
![shared-responsibility-model](/img/shared-responsibility-model.png)

##### Shared Responsibilities
Some responsibilities are shared, depending on the service and use case:
- AWS manages infrastructure-level encryption, but you manage application-level encryption.
- AWS offers compliance certifications, but you need to ensure your workloads follow them.

![Comparison](/img/security-share-responsibilty.png)

##### Different Ways of Provisioning and Operating in the AWS Cloud
AWS offers several methods for provisioning and managing resources:
- AWS Management Console
  - A web-based GUI to interact with AWS services.
  - Best for beginners and manual operations.
- AWS CLI (Command Line Interface)
  - Text-based tool to script and automate tasks.
  - Useful for developers and admins who prefer terminal-based control.
- AWS CloudShell – Browser-based shell preconfigured with CLI tools.
- AWS Tools for PowerShell – For Windows users to script AWS tasks.
- Programmatic Access via APIs and Lambda functions.
- AWS SDKs (Software Development Kits)
  - Libraries available for languages like Python (Boto3), JavaScript, Java, etc.
  - Ideal for integrating AWS into applications programmatically.
- AWS CloudFormation
  - Infrastructure as Code (IaC) tool to define AWS resources in JSON or YAML.
  - Great for replicable, consistent deployments.
- AWS CDK (Cloud Development Kit)
  - Define infrastructure using familiar programming languages like TypeScript or Python.
  - Combines IaC with real code logic.
- Terraform (by HashiCorp)
  - Third-party IaC tool, cloud-agnostic.
  - Popular for managing infrastructure across multiple cloud providers.
- AWS Systems Manager
  - Provides operational insights and automation tools for managing resources securely at scale.

##### Connectivity Options
Several ways to connect to AWS resources:
- Internet Access (Public endpoints)
  - Using the internet to access AWS services like S3, EC2.
- Virtual Private Network (VPN)
  - Secure connection between on-premises and AWS over the internet.
- AWS Direct Connect
  - Dedicated, private network connection to AWS.
  - Lower latency and more secure than VPN.
- VPC Peering
  - Connects two VPCs for communication.
- AWS Transit Gateway
  - Central hub to connect multiple VPCs and on-premises networks.
- Elastic Load Balancing (ELB)
  - Automatically distributes incoming application traffic.
- AWS PrivateLink
  - Private connectivity to AWS services without using public IPs.

##### Compliance and Governance concepts
AWS compliance and governance concepts, benefits of cloud security, and how to handle logs related to cloud security:

##### AWS Compliance and Governance Concepts
- Shared Responsibility Model
  - AWS manages security of the cloud (hardware, software, networking).
  - Customers manage security in the cloud (data, access, applications).
- Compliance Programs
  - AWS supports a broad set of industry certifications (e.g., HIPAA, PCI-DSS, SOC 1/2/3, ISO 27001).
  - AWS Artifact provides on-demand access to compliance reports.
- Governance Tools
  - AWS Organizations – Manage and govern multiple AWS accounts.
  - Service Control Policies (SCPs) – Set permission guardrails.
  - AWS Config – Track resource configurations and compliance over time.
  - AWS Control Tower – Automates landing zone setup with built-in governance.

##### Benefits of Cloud Security - Encryption
- Data Protection
  - Encryption at rest and in transit (via AWS KMS, TLS, etc.).
  - Automatic key rotation and policy enforcement.
- Scalability and Flexibility
  - Security tools scale with your infrastructure.
  - Integrates with services like Amazon GuardDuty and Amazon Inspector for threat detection.
- Identity and Access Management
  - AWS IAM for fine-grained access control.
  - MFA and role-based access enhance security posture.
- Continuous Monitoring
  - Real-time visibility with CloudWatch, CloudTrail, and AWS Security Hub.

##### Cloud Security Logs
- [AWS CloudTrail](https://docs.aws.amazon.com/cloudtrail/)
  It's a service that records and monitors actions taken in your AWS account, providing a history of API calls and user activity.
  - Logs all API calls and account activity across services.
  - Useful for auditing, compliance, and incident response.
  - Stored in S3, can be analyzed with Athena or CloudWatch Logs Insights.
- [Amazon CloudWatch](https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/cloudwatch_architecture.html)
  It's a monitoring service for Amazon Web Services (AWS) cloud resources and applications. It collects data, including metrics, logs, and events, to provide a comprehensive view of resource utilization, application performance, and operational health, according to Amazon AWS. 
  - Monitors logs, metrics, and events.
  - Collects application logs, system logs, and custom logs.
  - Enables setting alarms and automated responses.
- [VPC Flow Logs](https://docs.aws.amazon.com/vpc/latest/userguide/flow-logs.html)
  Flow log data can be published to the following locations: Amazon CloudWatch Logs, Amazon S3, or Amazon Data Firehose.
  - Capture network traffic metadata.
  - Useful for diagnosing network issues or detecting suspicious activity.
- [AWS Config](https://docs.aws.amazon.com/controltower/latest/userguide/config.html)
  AWS Config provides a detailed view of the resources associated with your AWS account, including how they are configured, how they are related to one another, and how the configurations and their relationships have changed over time.
  - Logs changes to resource configurations.
  - Useful for compliance monitoring and audit trails.
- [Amazon GuardDuty](https://docs.aws.amazon.com/AmazonRDS/latest/AuroraUserGuide/guard-duty-rds-protection.html)
  Amazon GuardDuty uses AI and ML with integrated threat intelligence from AWS and leading third parties to help protect your AWS accounts, workloads, and data from threats.
  - Threat detection service that generates security findings from logs.
  - Pulls from VPC Flow Logs, CloudTrail, and DNS logs.

##### [Network Access Control List (ACL)](https://docs.aws.amazon.com/vpc/latest/userguide/vpc-network-acls.html)
A network access control list (ACL) allows or denies specific inbound or outbound traffic at the subnet level. You can use the default network ACL for your VPC, or you can create a custom network ACL for your VPC with rules that are similar to the rules for your security groups in order to add an additional layer of security to your VPC.

##### [Web Application Firewall (WAF)](https://docs.aws.amazon.com/AmazonCloudFront/latest/DeveloperGuide/distribution-web-awswaf.html)
AWS WAF is a web application firewall that helps secure your web applications and APIs by blocking requests before they reach your servers. For more information, see Accelerate and protect your websites using CloudFront and AWS WAF and Guidelines for Implementing AWS WAF.

##### Firewalls & [Distributed Denial of Service (DDoS) Protection](https://aws.amazon.com/shield/ddos-attack-protection/)
- A firewall is a security system (hardware, software, or both) that monitors and controls incoming and outgoing network traffic based on predetermined security rules. To act as a barrier between a trusted internal network and untrusted external networks (like the internet), blocking malicious traffic.
- DDoS attacks attempt to overwhelm a network, server, or service with massive traffic from multiple sources to make it unavailable to legitimate users. To detect, mitigate, and recover from DDoS attacks before they cause downtime or service degradation.
##### 🔥 Firewall vs. 🌐 DDoS Protection
| Feature/Aspect              | 🔥 **Firewall**                               | 🌐 **DDoS Protection**                          |
| --------------------------- | -------------------------------------------- | ---------------------------------------------- |
| **Primary Function**        | Controls & filters network traffic           | Detects & mitigates traffic floods             |
| **Main Goal**               | Prevent unauthorized access                  | Maintain service availability during attacks   |
| **Type of Threats Handled** | Malware, intrusions, unauthorized access     | Volume-based, protocol, and app-layer attacks  |
| **Traffic Analysis**        | Packet inspection (rules, policies)          | Behavior & pattern analysis (attack detection) |
| **Deployment**              | Network perimeter, host-based, cloud         | Cloud-based, edge network, inline appliances   |
| **Can Stop DDoS?**          | ❌ Not reliably (can be overwhelmed)          | ✅ Yes, specifically designed for that          |
| **Stateful Tracking**       | Yes (for stateful firewalls)                 | Not typically, focuses on anomaly patterns     |
| **Real-Time Adaptation**    | Limited (static rules/policies)              | Advanced (dynamic mitigation, auto-scaling)    |
| **Best Use Case**           | Network access control and filtering         | Protecting against service downtime            |
| **Complementary?**          | ✅ Yes, part of overall security architecture | ✅ Yes, enhances firewall resilience            |

#### 03-domain-cloud-technology-services
This is the **largest domain** on the AWS Certified Cloud Practitioner (CLF-C02) exam, focusing on **core AWS services** and how they enable businesses to build, deploy, and operate applications in the cloud.

##### [AWS Compute Services](https://aws.amazon.com/products/compute/)
AWS offers a wide range of compute services for diverse workloads, from virtual servers to serverless functions and container orchestration. Key services include Amazon `EC2 (Elastic Compute Cloud)`, AWS `Fargate`, AWS `Lambda`, Amazon `ECS (Elastic Container Service)` and Amazon `EKS (Elastic Kubernetes Service)`, along with other specialized services like `AWS Batch` and `Lightsail`. 

###### AWS Lambda vs AWS Fargate
| Feature                | **AWS Lambda**                   | **AWS Fargate**                         |
| ---------------------- | -------------------------------- | --------------------------------------- |
| **Use Case**           | Event-driven, short tasks        | Containerized apps, long-running tasks  |
| **Runtime**            | Managed by AWS runtimes          | Custom Docker containers                |
| **Startup Time**       | Very fast (cold starts possible) | Slower (container startup time)         |
| **Max Execution Time** | 15 minutes                       | No hard limit                           |
| **Stateful?**          | Stateless                        | Can be stateful (with volumes like EFS) |
| **Billing**            | Per request + GB-seconds         | Per vCPU + memory per second            |
| **Infrastructure**     | Fully managed                    | More control (networking, IAM, etc.)    |
| **Scaling**            | Auto-scales instantly            | Scales well (slower than Lambda)        |

###### Amazon Lightsail vs AWS Elastic Beanstalk
| **Feature**                         | **Amazon Lightsail**                                          | **AWS Elastic Beanstalk**                                      |
| ----------------------------------- | ------------------------------------------------------------- | -------------------------------------------------------------- |
| **Target Audience**                 | Developers looking for simplicity, small businesses, startups | Developers requiring more flexibility and scaling options      |
| **Infrastructure Control**          | Minimal control, focuses on ease of use                       | More control over the infrastructure and configurations        |
| **Pricing**                         | Fixed, predictable pricing plans                              | Pay-as-you-go (EC2 instances, storage, etc.)                   |
| **Ease of Use**                     | Very easy to use, minimal configuration required              | Easy to use, but requires some understanding of AWS services   |
| **Scalability**                     | Limited scalability for larger apps                           | Autoscaling for high availability and large-scale apps         |
| **Customizability**                 | Limited customizability                                       | High degree of customization and configuration                 |
| **Supported Applications**          | Simple web apps, static sites, small applications             | Web apps, microservices, enterprise applications               |
| **Supported Programming Languages** | Limited to pre-configured stacks (e.g., LAMP, Node.js)        | Supports multiple programming languages and frameworks         |
| **Integration with AWS**            | Limited to Lightsail-specific features (e.g., S3, RDS)        | Full integration with AWS services (e.g., RDS, S3, CloudWatch) |

###### EC2 Instances Purchasing Options
|  SL   | Instance Name         |   Period   | Description                                                |
| :---: | :-------------------- | :--------: | :--------------------------------------------------------- |
|   1   | On-Demand             | Short Time | short workload, predictable pricing, pay by second         |
|   1   | Reserved Instances    | 1-3 Years  | long workloads with flexible instances                     |
|   2   | Savings Plans         | 1-3 Years  | commitment to an amount of usage, long workload            |
|   3   | Spot Instances        | Short Time | short workloads, cheap, can lose instances (less reliable) |
|   4   | Dedicated Hosts       | Long Time  | book an entire physical server, control instance placement |
|   5   | Dedicated Instances   |    N/A     | no other customers will share your hardware                |
|   6   | Capacity Reservations |    N/A     | reserve capacity in a specific AZ for any duration         |

##### [AWS Database Service](https://docs.aws.amazon.com/whitepapers/latest/aws-overview/database.html)
AWS offers a wide range of database services, covering everything from traditional relational databases to modern NoSQL, in-memory, and graph databases. Here's a breakdown of the major ones by type:
- Relational Databases (SQL)
  - [Amazon RDS (Relational Database Service)](https://aws.amazon.com/rds/?p=ft&c=db&z=3)
    - Fully managed database service for SQL-based engines.
    - Supports: MySQL, PostgreSQL, MariaDB, Oracle, SQL Server, Aurora.
    - Handles backups, patching, scaling, etc.
  - [Amazon Aurora](https://aws.amazon.com/rds/aurora/)
    - High-performance, cloud-native relational database.
    - Compatible with MySQL and PostgreSQL.
    - Up to 5x faster than standard MySQL, with built-in replication and high availability.
    - Serverless version: Aurora Serverless v2 (auto-scales capacity).
- NoSQL Databases
  - Amazon DynamoDB
    - Fully managed key-value and document NoSQL database.
    - Ultra-fast, scalable, and serverless.
    - Ideal for real-time apps, gaming, IoT, serverless apps.
  - Amazon ElastiCache
    - In-memory caching service.
    - Supports: Redis and Memcached.
    - Great for speeding up apps with frequently accessed data (e.g., sessions, leaderboards).
- Amazon Keyspaces (for Apache Cassandra)
  - Managed Cassandra-compatible NoSQL database.
  - Serverless and scalable.
- Graph, Time Series, and Ledger
  - Amazon Neptune
    - Graph database for highly connected data.
    - Supports: Gremlin and SPARQL.
    - Use cases: social networks, recommendation engines, fraud detection.

###### Comparison of Amazon RDS vs Amazon Aurora
| Feature                  | Amazon RDS                                     | Amazon Aurora                                         |
| ------------------------ | ---------------------------------------------- | ----------------------------------------------------- |
| **Engine Compatibility** | MySQL, PostgreSQL, MariaDB, Oracle, SQL Server | MySQL, PostgreSQL                                     |
| **Performance**          | Standard performance                           | Up to 5x faster than MySQL, 2x faster than PostgreSQL |
| **Availability**         | Multi-AZ deployment option                     | Multi-AZ replication, automatic failover              |
| **Storage Scaling**      | Scalable storage (up to 16 TB)                 | Automatic scaling up to 128 TB                        |
| **Cost**                 | Generally lower cost                           | Higher cost, but higher performance and scalability   |
| **Backup & Recovery**    | Automated backups with point-in-time recovery  | Continuous backups to S3, point-in-time recovery      |
| **Replication**          | Read replicas available (varies by engine)     | Aurora Replicas, up to 15 replicas                    |

##### [DNS, Networking and content delivery](https://docs.aws.amazon.com/whitepapers/latest/aws-overview/networking-services.html)
AWS offers a broad set of networking and content delivery services that provide the highest level of reliability, security, and performance in the cloud.
###### [Amazon API Gateway](https://docs.aws.amazon.com/whitepapers/latest/aws-overview/networking-services.html)
###### [Amazon CloudFront](https://docs.aws.amazon.com/whitepapers/latest/aws-overview/networking-services.html)
###### [Amazon Route 53](https://docs.aws.amazon.com/whitepapers/latest/aws-overview/networking-services.html)
Amazon Route 53 is a scalable and highly available Domain Name System (DNS) web service by AWS. A Route 53 record (or DNS record) is used to define how you want to route traffic for a domain or subdomain. Here's a quick breakdown of what you need to know:

DNS Record
| Record Type | Purpose                                                     |
| ----------- | ----------------------------------------------------------- |
| A           | Maps a domain to an IPv4 address.                           |
| AAAA        | Maps a domain to an IPv6 address.                           |
| CNAME       | Maps a domain to another domain (used for aliasing).        |
| MX          | Specifies mail servers for email delivery.                  |
| TXT         | Holds arbitrary text (e.g., SPF, domain verification).      |
| NS          | Lists authoritative name servers for the domain.            |
| SOA         | Start of Authority – provides info about the domain/zone.   |
| SRV         | Specifies location of services (e.g., SIP, XMPP).           |
| Alias       | AWS-specific alias to AWS resources (e.g., S3, CloudFront). |

A Record Example
| Record Type | Value           |
| ----------- | --------------- |
| Name:       | www.example.com |
| Type:       | A               |
| Value       | : 54.123.45.67  |
| TTL:        | 300 (seconds)   |

Alias Record Example
| Record Type     | Value                |
| --------------- | -------------------- |
| Name:           | example.com          |
| Type:           | A (Alias)            |
| Alias Target:   | d1234.cloudfront.net |
| Routing Policy: | Simple               |

###### [Amazon VPC](https://docs.aws.amazon.com/whitepapers/latest/aws-overview/networking-services.html)
###### [AWS VPN](https://docs.aws.amazon.com/whitepapers/latest/aws-overview/networking-services.html)
###### [Elastic Load Balancing](https://docs.aws.amazon.com/whitepapers/latest/aws-overview/networking-services.html)
Load balancers are servers that forward internet traffic to multiple servers (EC2 Instances) downstream.
![Load Balancing](/img/load-balancing.png)

**Why use a load balancer?**
- Spread load across multiple downstream instances
- Expose a single point of access (DNS) to your application
- Seamlessly handle failures of downstream instances
- Do regular health checks to your instances
- Provide SSL termination (HTTPS) for your websites
- High availability across zones

**Why use an Elastic Load Balancer?**
- An ELB (Elastic Load Balancer) is a managed load balancer.
  - AWS guarantees that it will be working
  - AWS takes care of upgrades, maintenance, high availability
  - AWS provides only a few configuration knobs
- It costs less to setup your own load balancer but it will be a lot more effort on your end (maintenance, integrations)
- 4 kinds of load balancers offered by AWS:
  - Application Load Balancer (HTTP / HTTPS only) – Layer 7 (APS TNDP)
    - 7 Layer (Application > Presentation > Session > Transport > Network > Data Link > Physical)
  - Network Load Balancer (ultra-high performance, allows for TCP) – Layer 4
    - 4 Layer (Application > Transport > Internet > Network)
  - Gateway Load Balancer – Layer 3
  - Classic Load Balancer (retired in 2023) – Layer 4 & 7
![Elastic Load Balancer](/img/elastic-load-balancer.png)

**What’s an Auto Scaling Group?**
- In real-life, the load on your websites and application can change
- In the cloud, you can create and get rid of servers very quickly
- The goal of an Auto Scaling Group (ASG) is to:
- Scale out (add EC2 instances) to match an increased load
- Scale in (remove EC2 instances) to match a decreased load
- Ensure we have a minimum and a maximum number of machines running
- Automatically register new instances to a load balancer
- Replace unhealthy instances
- Cost Savings: only run at an optimal capacity (principle of the cloud)

**Auto Scaling Group**
![Auto Scaling Group](/img/auto-scaling-group.png)

**Auto Scaling Group with Load Balancer**
![Auto Scaling Group with Load Balancer](/img/auto-scaling-group-load-balancer.png)

**Difference between Load Balancer and Auto Scaling**
|    Factors     | Load Balancer                   | Auto Scaling                    |
| :------------: | :------------------------------ | :------------------------------ |
|    Purpose     | Distribute the incoming traffic | Adjust the number of resources  |
| Algorithm used | Round-Robin algorithm or least  | Step Scaling or Target Tracking |

**Security Groups (SG)**
- Security Groups are the fundamental of network security in AWS. Its working like as firewall.
- They control how traffic is allowed into or out of our EC2 Instances. Inbound traffic
- Security groups only contain rules
- Security groups rules can reference by IP or by security group.

Illustration shown as follows;
![Security Group](/img/security-group.png)

**Security Groups Deeper Dive**
- Security groups are acting as a “firewall” on EC2 instances
- They regulate:
  - Access to Ports
  - Authorized IP ranges – IPv4 and IPv6
  - Control of inbound network (from other to the instance)
  - Control of outbound network (from the instance to other)

Illustration shown as follows;
![Security Group Details](/img/sg-details.png)

Security Group Diagram
Illustration shown as follows;
![Security Group Diagram](/img/sg-diagram.png)

**Security Groups Good to know**
- Can be attached to multiple instances
- Locked down to a region / VPC combination
- Does live “outside” the EC2 – if traffic is blocked the EC2 instance won’t see it
- It’s good to maintain one separate security group for SSH access
- If your application is not accessible (time out), then it’s a security group issue
- If your application gives a “connection refused“ error, then it’s an application error or it’s not launched
- All inbound traffic is blocked by default
- All outbound traffic is authorized by default

**SG Diagram Ref Other SG** Illustration shown as follows;
![SG Diagram Ref Other SG](/img/sg-diagram-ref-other-sg.png)

**Some important Port**
|  SL   | Port | Protocol                      |
| :---: | :--- | :---------------------------- |
|   1   | 21   | FTP                           |
|   2   | 22   | SSH                           |
|   3   | 22   | SFTP                          |
|   4   | 80   | HTTP                          |
|   5   | 443  | HTTPS                         |
|   6   | 3389 | Remote Desktop Protocol (RDP) |

###### [AWS Direct Connect](https://docs.aws.amazon.com/whitepapers/latest/aws-overview/networking-services.html)
###### [AWS Global Accelerator](https://docs.aws.amazon.com/whitepapers/latest/aws-overview/networking-services.html)
###### [AWS PrivateLink](https://docs.aws.amazon.com/whitepapers/latest/aws-overview/networking-services.html)
###### [AWS Private 5G](https://docs.aws.amazon.com/whitepapers/latest/aws-overview/networking-services.html)
###### [AWS Transit Gateway](https://docs.aws.amazon.com/whitepapers/latest/aws-overview/networking-services.html)
###### [Integrated Private Wireless on AWS](https://docs.aws.amazon.com/whitepapers/latest/aws-overview/networking-services.html)

##### [Security, identity, and compliance](https://docs.aws.amazon.com/whitepapers/latest/aws-overview/security-services.html)
###### [Amazon Cognito](https://docs.aws.amazon.com/whitepapers/latest/aws-overview/security-services.html)
###### [Amazon Detective](https://docs.aws.amazon.com/whitepapers/latest/aws-overview/security-services.html)
###### [Amazon GuardDuty](https://docs.aws.amazon.com/whitepapers/latest/aws-overview/security-services.html)
###### [Amazon Inspector](https://docs.aws.amazon.com/whitepapers/latest/aws-overview/security-services.html)
###### [Amazon Macie](https://docs.aws.amazon.com/whitepapers/latest/aws-overview/security-services.html)
###### [Amazon Security Lake](https://docs.aws.amazon.com/whitepapers/latest/aws-overview/security-services.html)
###### [Amazon Verified Permissions](https://docs.aws.amazon.com/whitepapers/latest/aws-overview/security-services.html)
###### [AWS Artifact](https://docs.aws.amazon.com/whitepapers/latest/aws-overview/security-services.html)
###### [AWS Audit Manager](https://docs.aws.amazon.com/whitepapers/latest/aws-overview/security-services.html)
###### [AWS Certificate Manager](https://docs.aws.amazon.com/whitepapers/latest/aws-overview/security-services.html)
###### [AWS CloudHSM](https://docs.aws.amazon.com/whitepapers/latest/aws-overview/security-services.html)
###### [AWS Directory Service](https://docs.aws.amazon.com/whitepapers/latest/aws-overview/security-services.html)
###### [AWS Firewall Manager](https://docs.aws.amazon.com/whitepapers/latest/aws-overview/security-services.html)
###### [AWS Identity and Access Management](https://docs.aws.amazon.com/whitepapers/latest/aws-overview/security-services.html)
###### [AWS Key Management Service](https://docs.aws.amazon.com/whitepapers/latest/aws-overview/security-services.html)
###### [AWS Network Firewall](https://docs.aws.amazon.com/whitepapers/latest/aws-overview/security-services.html)
###### [AWS Resource Access Manager](https://docs.aws.amazon.com/whitepapers/latest/aws-overview/security-services.html)
###### [AWS Secrets Manager](https://docs.aws.amazon.com/whitepapers/latest/aws-overview/security-services.html)
###### [AWS Security Hub](https://docs.aws.amazon.com/whitepapers/latest/aws-overview/security-services.html)
###### [AWS Shield](https://docs.aws.amazon.com/whitepapers/latest/aws-overview/security-services.html)
###### [AWS IAM Identity Center](https://docs.aws.amazon.com/whitepapers/latest/aws-overview/security-services.html)
###### [AWS WAF](https://docs.aws.amazon.com/whitepapers/latest/aws-overview/security-services.html)
###### [AWS WAF Captcha](https://docs.aws.amazon.com/whitepapers/latest/aws-overview/security-services.html)

##### [AWS Storage Services](https://docs.aws.amazon.com/whitepapers/latest/aws-overview/storage-services.html)
There are three types of storage in Amazon Web Services
1. Object Storage
   - S3 Storage
   - S3 Glacier Storage
   - Snowball Storage
2. File Storage
   - Elastic File System (EFS)
   - FSx Storage (Windows)
   - FSx Storage (Lustre)
3. Block Storage
   - [Elastic Block Storage (EBS)](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ebs-volume-types.html)
     - SSD Storage volumes
       - General Purpose (GP2) volumes
       - Provisioned IOPS SSD (io1) volumes
       - Provisioned IOPS SSD (io2) volumes
     - HDD Storage
       - Throughput Optimized (ST1)
       - Cold HDD (SC1)
     - Magnetic Storage
   - EC2 Instance Storage

###### IOPS (eye-ops):
Input/Output Operation per Second is use as I/O performance management measurement to characterize computer storage devices like HDD, SSD & Storage Area Network (SAN). This Operations (reads or writes) that a storage system can perform in one second. It focuses on the speed at which individual read and write operations can be completed. Its measure in KiB.
- Maximum amount of data that a volume type counts as 'Single I/O'.
- I/O size capped at 256 KiB for SSD.
- I/O size capped at 1024 KiB for HDD.
- SSD volumes handle small/random I/O more efficiently than HDD volumes.

###### IOPS Calculation:
Average Seek Time = (Read Time + Write Time)/2
IOPS = 1 / (RPM Average Latency Time + Average Seek Time)
Suppose, Rotational Speed = 15,000, RPM Average Latency Time = 3 ms = 0.003 Seconds, Average Seek Time = {4.2 (R) + 4.45 (W)}/2 = 4.45 ms = 0.0045 Second

IOPS = 1 / (0.003 + 0.0045) = 133 IOPS (Approximately)

###### Throughput
Its refers to the rate at which data is transferred successfully between two points in a system, such as between a storage device and a server, or within a network. Throughput can be affected by IOPS & packet size.

##### Each type of storage is discussed in detail that is as follows;
###### [1.1- Object Storage (S3 Storage)](https://aws.amazon.com/pm/serv-s3/?trk=b8b87cd7-09b8-4229-a529-91943319b8f5&sc_channel=ps&ef_id=CjwKCAiA_aGuBhACEiwAly57MX61bi-mAlAD0os3_jPx0l3oYV-mkTDNdI8gy4MVE8cY776K1fRZxRoCi6gQAvD_BwE:G:s&s_kwcid=AL!4422!3!536456067065!e!!g!!s3%20storage!11539706604!115473954914&gclid=CjwKCAiA_aGuBhACEiwAly57MX61bi-mAlAD0os3_jPx0l3oYV-mkTDNdI8gy4MVE8cY776K1fRZxRoCi6gQAvD_BwE)
It is an object storage service offering industry-leading scalability, data availability, security, and performance.
**Uses of S3**  (as like Google Drive, One Drive, Drop Box etc.)
- Backup and storage
- Disaster Recovery
- Archive
- Hybrid Cloud storage
- Application hosting
- Media hosting
- Data lakes & big data analytics
- Software delivery
- Static website

**Buckets**
- Amazon S3 allows people to store objects (files) in “buckets” (directories)
- Buckets must have a globally unique name (across all regions all accounts)
- Buckets are defined at the region level
- S3 looks like a global service but buckets are created in a region
  - Naming convention
  - No uppercase, No underscore
  - 3-63 characters long
  - Not an IP
  - Must start with lowercase letter or number
  - Must NOT start with the prefix xn--
  - Must NOT end with the suffix -s3alias

**Objects**
- Objects (files) have a Key
- The key is the FULL path:
  - s3://my-bucket/my_file.txt
  - s3://my-bucket/my_folder1/another_folder/my_file.txt
- The key is composed of prefix + object name
  - s3://my-bucket/my_folder1/another_folder/my_file.txt
- There’s no concept of “directories” within buckets (although the UI will trick you to think otherwise)
- Just keys with very long names that contain slashes (“/”)
- Object values are the content of the body:
  - Max. Object Size is 5TB (5000GB)
  - If uploading more than 5GB, must use “multi-part upload”
- Metadata (list of text key / value pairs – system or user metadata)
- Tags (Unicode key / value pair – up to 10) – useful for security / lifecycle
- Version ID (if versioning is enabled)

**Security**
- User-Based
  - IAM Policies – which API calls should be allowed for a specific user from IAM
- Resource-Based
  - Bucket Policies – bucket wide rules from the S3 console - allows cross account
  - Object Access Control List (ACL) – finer grain (can be disabled)
  - Bucket Access Control List (ACL) – less common (can be disabled)
- Note: an IAM principal can access an S3 object if
  - The user IAM permissions ALLOW it OR the resource policy ALLOWS it
  - AND there’s no explicit DENY
- Encryption: encrypt objects in Amazon S3 using encryption keys

**S3 Bucket Policies**
- JSON based policies
  - Resources: buckets and objects
  - Effect: Allow / Deny
  - Actions: Set of API to Allow or Deny
  - Principal:The account or user to apply the policy to
- Use S3 bucket for policy to:
  - Grant public access to the bucket
  - Force objects to be encrypted at upload
  - Grant access to another account (Cross Account)

Example (S3 Bucket Policies)
```JSON
{
  "Version": "2024-02-12",
  "Statement": [
    {
      "Sid": "PublicRead",
      "Effect": "Allow",
      "Principal": "*",
      "Action": [
        "s3:GetObject"
      ],
      "Resource": [
        "arn:aws:s3:::my_sweet_bucket/*"
      ]
    }
  ]
}
```

###### [1.2- Object Storage (S3 Glacier Storage)](https://aws.amazon.com/pm/s3-glacier/?trk=b8b87cd7-09b8-4229-a529-91943319b8f5&sc_channel=ps&ef_id=CjwKCAiA_aGuBhACEiwAly57Mdp21CgKnEvgufcIeYZ_cnX3_6l4342RMJhP5OBESh-aP2g1mjr_dBoCxecQAvD_BwE:G:s&s_kwcid=AL!4422!3!674509861659!e!!g!!amazon%20s3%20glacier!11539706604!154273570032&gclid=CjwKCAiA_aGuBhACEiwAly57Mdp21CgKnEvgufcIeYZ_cnX3_6l4342RMJhP5OBESh-aP2g1mjr_dBoCxecQAvD_BwE)
- The Amazon S3 Glacier storage classes are purpose-built for data archiving, providing you with the highest performance, most retrieval flexibility, and the lowest cost archive storage in the cloud.
- Choose from three archive storage classes optimized for different access patterns and storage duration.
- The S3 Glacier storage classes provide virtually unlimited scalability and are designed for 99.999999999% (11 nines) of data durability.

###### [1.3- Object Storage (Snowball Storage)](https://aws.amazon.com/snowball/)
Accelerate moving offline data or remote storage to the cloud. Description: Snowball is a petabyte-scale data transport solution that uses secure appliances to transfer large amounts of data into and out of the AWS cloud. Using Snowball addresses common challenges with large-scale data transfers including high network costs, long transfer times, and security concerns.
Features:
- A service fee for each job you run, 
- Data transfer fees from Amazon S3,
- The shipping costs to transport a Snowball appliance to and from your address, and 
- The number of days you keep Snowball onsite. [For details](https://aws.amazon.com/snowball/pricing/)

###### 2.1- File Storage [Elastic File System (EFS)]
**EFS Infrequent Access (EFS-IA)**
- Managed NFS (network file system) that can be mounted on 100s of EC2
- EFS works with Linux EC2 instances in multi-AZ
- Highly available, scalable, expensive (3x gp2), pay per use, no capacity planning
- Storage class that is cost-optimized for files not accessed every day
- Up to 92% lower cost compared to EFS Standard
- EFS will automatically move your files to EFS-IA based on the last time they were accessed
- Enable EFS-IA with a Lifecycle Policy
- Example: move files that are not accessed for 60 days to EFS-IA
- Transparent to the applications accessing EFS
- cost-optimized storage class for infrequent accessed files

###### 2.2- File Storage [FSx Storage (Windows)]
Launch 3rd party high-performance file systems on AWS. Fully managed service
- A fully managed, highly reliable, and scalable Windows native shared file system
- Built on Windows File Server
- Supports SMB protocol & Windows NTFS
- Integrated with Microsoft Active Director y
- Can be accessed from AWS or your on-premise infrastructure
- Network File System for Windows servers

###### 2.3- File Storage [FSx Storage (Lustre)]
- A fully managed, high-performance, scalable file storage for High Performance Computing (HPC)
- The name Lustre is derived from “Linux” and “cluster”
- Machine Learning, Analytics,Video Processing, Financial Modeling, ...
- Scales up to 100s GB/s, millions of IOPS, sub-ms latencies

###### 3.1- Block Storage [Elastic Block Storage (EBS)]
An EBS (Elastic Block Store) Volume is a network drive (i.e. not a physical drive) you can attach to your instances while they run
- It allows your instances to persist data, even after their termination
- They can only be mounted to one instance at a time (at the Certified Cloud Practitioner (CCP) level)
- They are bound to a specific availability zone
- Analogy:Think of them as a “network USB stick”
- Free tier: 30 GB of free EBS storage of type General Purpose (SSD) or Magnetic per month
- It uses the network to communicate the instance, which means there might be a bit of latency
- It can be detached from an EC2 instance and attached to another one quickly
- It’s locked to an Availability Zone (AZ)
- An EBS Volume in ***us-east-1a*** cannot be attached to ***us-east-1b***
- To move a volume across, you first need to snapshot it
- Have a provisioned capacity (size in GBs, and IOPS)
- You get billed for all the provisioned capacity
- You can increase the capacity of the drive over time

- **EBS Snapshots Features**
  - EBS Snapshot Archive
    - Move a Snapshot to an ”archive tier” that is 75% cheaper
    - Takes within 24 to 72 hours for restoring the archive
  - Recycle Bin for EBS Snapshots
    - Setup rules to retain deleted snapshots so you can recover them after an accidental deletion
    - Specify retention (from 1 day to 1 year)

###### [3.2 Block Storage (EC2 Instance Storage)](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/InstanceStorage.html)
An instance store provides temporary block-level storage for your instance. This storage is located on disks that are physically attached to the host computer. Instance store is ideal for temporary storage of information that changes frequently, such as buffers, caches, scratch data, and other temporary content. It can also be used to store temporary data that you replicate across a fleet of instances, such as a load-balanced pool of web servers.
Features:
An instance store consists of one or more instance store volumes exposed as block devices. The size of an instance store as well as the number of devices available varies by instance type and instance size. [For more](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/InstanceStorage.html)

- **Amazon Machine Image (AMI)**
  - AMI are a customization of an EC2 instance
    - You add your own software, configuration, operating system, monitoring... 
    - Faster boot/configuration time because all your software is pre-packaged
  - AMI are built for a specific region (and can be copied across regions)
  - You can launch EC2 instances from:
    - A Public AMI: AWS provided
    - Your own AMI: you make and maintain them yourself
    - An AWS Marketplace AMI: an AMI someone else made (and potentially sells)

- **AMI Process (from an EC2 instance)**
  - Start an EC2 instance and customize it
  - Stop the instance (for data integrity)
  - Build an AMI – this will also create EBS snapshots 
  - Launch instances from other AMIs

- **EC2 Image Builder**
  - Used to automate the creation ofVirtual Machines or container images
  - Automate the creation, maintain, validate and test EC2 AMIs
  - Can be run on a schedule (weekly, whenever packages are updated, etc...)
  - Free service (only pay for the underlying resources)
Illustration shown below;
![Image builder](/img/image-builder.png)

###### Shared Responsibility Model of Storage Volume
| AWS (Provider)                                    | User                                               |
| :------------------------------------------------ | :------------------------------------------------- |
| Infrastructure                                    | Setting up backup / snapshot procedures            |
| Replication for data for EBS volumes & EFS drives | Setting up data encryption                         |
| Replacing faulty hardware                         | Responsibility of any data on the drives           |
| Ensuring their employees cannot access your data  | Understanding the risk of using EC2 Instance Store |

###### Services from other in-scope AWS Service Categories
- Application Integration Services
  These services help applications communicate and process events or messages reliably.
  - Amazon EventBridge: Event bus for building event-driven applications at scale.
  - Amazon SNS (Simple Notification Service): Pub/sub messaging for decoupled microservices.
  - Amazon SQS (Simple Queue Service): Managed message queuing for distributed systems.
- Business Application Services
  Enable customer service and communication workflows.
  - Amazon Connect: Cloud-based contact center service.
  - Amazon SES (Simple Email Service): Scalable email sending for marketing or transactional purposes.
- Customer Engagement Services
  These services support customer success and AWS account management.
  - AWS Activate for Startups: Credits, training, and support for startup growth.
  - AWS IQ: Connects customers with AWS-certified freelancers and consultants.
  - AWS Managed Services (AMS): Operational support and automation for AWS infrastructure.
  - AWS Support: Tiered support plans offering guidance and troubleshooting.
- Developer Tools
  Helps developers build, test, and deliver code quickly and securely.
  - AWS AppConfig: Feature flagging and configuration management.
  - AWS Cloud9: Cloud-based IDE for writing, running, and debugging code.
  - AWS CloudShell: Browser-based shell for command-line access to AWS.
  - AWS CodeArtifact: Artifact repository for software packages.
  - AWS CodeBuild: Continuous integration service to compile and test code.
  - AWS CodeCommit: Fully managed Git-based source control.
  - AWS CodeDeploy: Automates code deployments to compute services.
  - AWS CodePipeline: CI/CD pipeline orchestration tool.
  - AWS CodeStar: Unified interface for software development.
  - AWS X-Ray: Distributed tracing system for analyzing and debugging applications.
- End-User Computing Services
  Provides remote desktops and application streaming for users.
  - Amazon AppStream 2.0: Stream desktop apps to users over the web.
  - Amazon WorkSpaces: Managed virtual desktops in the cloud.
  - Amazon WorkSpaces Web: Secure browser access to internal websites and apps.
- Frontend Web and Mobile Services
  Helps developers build full-stack web and mobile applications.
  - AWS Amplify: Set of tools to build, ship, and host full-stack applications.
  - AWS AppSync: Managed GraphQL service for querying and syncing data in real-time.
- IoT Services
  Connect and manage IoT devices and edge computing.
  - AWS IoT Core: Secure device communication with cloud apps and services.
  - AWS IoT Greengrass: Brings AWS compute, messaging, and data caching to edge devices.

#### 04-domain-billing-pricing-support
##### AWS Pricing Fundamentals
AWS Pricing Fundamentals is something every AWS user should understand — it helps you use AWS more efficiently and avoid surprise bills. Let's break it down into key principles and pricing models.
- Pay-as-you-go
- You only pay for what you use.
- No upfront costs or long-term contracts (unless you choose them for savings).
- Pay less when you reserve
- Reserved Instances (RIs) or Savings Plans let you commit to usage over 1 or 3 years for big discounts (up to 72%).
- Pay less with more usage
- Some services have tiered pricing (like S3 and Data Transfer) — the more you use, the less you pay per unit.
- Free tier
- Many services include a free usage allowance for 12 months or always-free (e.g., Lambda, S3, DynamoDB, CloudWatch).

**AWS Pricing Models**
| Model             | Applies To                    | Description                                           |
| ----------------- | ----------------------------- | ----------------------------------------------------- |
| **On-Demand**     | EC2, RDS, Lambda, etc.        | Pay per use, flexible, no commitments                 |
| **Reserved**      | EC2, RDS, ElastiCache         | Commit for 1 or 3 years for big discounts             |
| **Savings Plans** | EC2, Lambda, Fargate          | up to 72%, Flexible alternative to Reserved Instances |
| **Spot**          | EC2                           | Up to 90% off for interruptible workloads             |
| **Tiered**        | S3, CloudFront, Data Transfer | Lower unit prices at higher usage volumes             |
| **Request-based** | Lambda, API Gateway, DynamoDB | Charged per request or execution                      |
| **Per-GB/IO**     | S3, EBS, Data Transfer        | Based on size or read/write operations                |

**Cost-Saving Tips**
- Use **Spot Instances** for fault-tolerant or test workloads.
- Reserve capacity with **Savings Plans** or **RIs** for predictable usage.
- Store infrequently accessed data in **S3 Infrequent Access** or **Glacier**.
- Use **Auto Scaling** to avoid idle resources.
- Monitor usage with **Cost Explorer** and set **budgets**.

###### [Core AWS Pricing Concepts](https://aws.amazon.com/economics/)
Cloud economics refers to the financial principles and business value derived from cloud computing. It helps organizations understand how to optimize costs, `improve return on investment (ROI)`, and maximize the value of cloud adoption.

##### Price of Cloud
AWS has 3 pricing fundamentals, following the pay-as-you-go pricing model
1. Compute: Pay for compute time
2. Storage: Pay for data stored in the Cloud
3. Data transfer out of the Cloud: Data transfer in is free
Its the expensive issue then traditional IT

###### BYOL (Bring Your Own License)?
BYOL is a licensing model that lets you use your existing software licenses (like Windows, SQL Server, Oracle, etc.) when migrating or deploying workloads on AWS. Instead of buying new licenses through AWS, you "bring" the ones you already own—usually through volume licensing agreements from Microsoft, Oracle, etc.

##### Amazon EC2 Pricing Use Cases
##### Pricing for other AWS Services
##### AWS Pricing Calculator - `HOL`
##### AWS Support Plans
##### Consolidated Billing
##### Cost Allocation Tags
##### AWS Cost Management Tools
##### AWS Cost Explorer - `HOL`


### [AWS Certified Cloud Practitioner - DVA-02](https://aws.amazon.com/certification/certified-cloud-practitioner/)
#### Exam Overview
| SL  | Title                   | Weight                              |
| --- | ----------------------- | ----------------------------------- |
| 1   | Exam Code:              | DVA-C02                             |
| 2   | Duration:               | 130 minutes                         |
| 3   | Fees:                   | 150 USD                             |
| 4   | Certification Validity: | 3 years                             |
| 5   | Format:                 | Multiple Choice & Multiple Response |
| 6   | Delivery:               | Pearson VUE or PSI                  |

#### Who Should Take the Exam Ideal for:
- Developers with **1+ Years** of experience with AWS
- DevOps Engineers, App Developers, Backend Engineers
- Anyone working with AWS services like Lambda, DynamoDB, S3, API Gateway, etc.

#### Exam Domains and Weightings
| SL  | Domain                           | Weight |
| --- | -------------------------------- | ------ |
| 1   | Development with AWS Services    | 32%    |
| 2   | Security                         | 26%    |
| 3   | Deployment                       | 24%    |
| 4   | Troubleshooting and Optimization | 18%    |

### [AWS Certified DevOps Engineer Professional - DOP-C02](https://aws.amazon.com/certification/certified-devops-engineer-professional/)
#### [DevOps Model](https://aws.amazon.com/devops/what-is-devops/)
DevOps is the combination of `cultural philosophies`, `practices`, and tools that increases an organization’s `ability to deliver applications` and services at `high velocity`: evolving and improving products at a faster pace than organizations using traditional software development and infrastructure management processes. This speed enables organizations to better serve their customers and compete more effectively in the market.
![DevOps Model](/img/devops.jpg)

#### How DevOps Works
Under a DevOps model, development and operations teams are no longer `siloed`. Sometimes, these two teams are merged into a single team where the engineers work across the entire application lifecycle, from development and test to deployment to operations, and develop a range of skills not limited to a single function.

In some DevOps models, quality assurance and security teams may also become more tightly integrated with development and operations and throughout the application lifecycle. When security is the focus of everyone on a DevOps team, this is sometimes referred to as DevSecOps.

These teams use practices to automate processes that historically have been manual and slow. They use a technology stack and tooling which help them operate and evolve applications quickly and reliably. These tools also help engineers independently accomplish tasks (for example, deploying code or provisioning infrastructure) that normally would have required help from other teams, and this further increases a team’s velocity.

#### Four Pillars of DevOps
- Automation
- Quality
- Monitoring
- Testing

#### Benefits of DevOps
- Speed
- Rapid Delivery
- Reliability
- Scale
- Improved Collaboration
- Security

#### Why DevOps Matters
DevOps matters because it directly impacts how fast, reliable, and efficiently a company can deliver software and services to its customers. In today’s world, where users expect seamless digital experiences and rapid innovation, DevOps helps organizations stay competitive. Here’s why DevOps really matters:
- Faster Time to Market
- Continuous Improvement & Delivery
- Improved Collaboration
- Better Quality and Fewer Bugs
- Scalability and Flexibility
- Enhanced Security
- Cost Efficiency
In conclusion, DevOps matters for several reasons, including faster and more reliable service delivery, reduced bugs, optimized speed, and cost control across all aspects of development and operations.

#### DevOps Cultural Philosophy
DevOps is an agile approach to organizational change that seeks to bridge traditional, siloed divides between teams and establish new processes that facilitate greater collaboration. At its essence, a DevOps culture involves closer collaboration and a shared responsibility between development and operations for the products they create and maintain. This helps companies align their people, processes, and tools toward a more unified customer focus. 

#### DevOps Practices
DevOps is all about the integration of development and operations through a set of best practices and principles that help streamline software development, deployment, and maintenance. These practices aim to achieve faster, more reliable, and efficient software delivery while fostering collaboration between teams. Here are some of the core DevOps practices that help organizations achieve their goals:
- Continuous Integration
- Continuous Delivery
- Microservices
- Infrastructure as Code
- Monitoring and Logging
- Communication and Collaboration
- Automated Testing

#### Benefits of DevOps Culture:
- Streamlined, frequent, and high-quality software releases.
- Improved company performance and employee satisfaction.
- Fosters trust and collaboration among teams.
- Leads to better decision-making and higher job satisfaction.
- Engineers experience the reward of deploying stable, high-performing software.
- Executives benefit from improved business outcomes.

#### Challenges:
- Significant changes in workflows and buy-in at all levels (especially from leadership) are required.
- Grassroots efforts can help demonstrate success and convince executives.
- Building trust and autonomy can be difficult if there’s a history of conflict or silos.
- Clear communication of the benefits of change is necessary for acceptance.
- Tool adoption without cultural change can lead to “cargo-cult DevOps”, which focuses on the facade but ignores the core issues.

#### What is Agile?
Agile is an `iterative and incremental approach` to project management and software development that focuses on `collaboration`, `customer feedback`, and `rapid releases`. Agile is mainly about developing software in `small`, `manageable pieces` while `maintaining flexibility` and a `strong focus` on customer needs. It’s about how the team works together to build software, how they adapt to changes, and how they deliver value quickly.

![Agile Methodology](/img/agile.png)

#### Agile Manifesto?
The Agile Manifesto is a foundational document that outlines the core values and principles of the Agile methodology. The Manifesto consists of `4` key values and `12` principles that guide Agile teams in their work. As outlined in the Agile Manifesto, there are `four` main values of Agile project management.

##### `Four` pillars of Agile?
- `Individuals over processes and tools.` Agile teams value team collaboration and teamwork over working independently and doing things "by the book.”
- `Working software over comprehensive documentation.` The software that Agile teams develop should work. Additional work, like documentation, is not as important as developing good software.
- `Customer collaboration over contract negotiation.` Customers are extremely important within the Agile methodology. Agile teams allow customers to guide where the software should go. Therefore, customer collaboration is more important than the finer details of contract negotiation.
- `Responding to change over following a plan.` One of the major benefits of Agile project management is that it allows teams to be flexible. This framework allows for teams to quickly shift strategies and workflows without derailing an entire project.

##### `Twelve` Agile principles?
If the four values of the Agile model are the weight-bearing pillars of a house, then the 12 Agile principles are the rooms you can build within that house. These principles can be easily adapted to fit the needs of your software development process. The 12 principles used in Agile methodology are:
- `Satisfy customers through early, continuous improvement and delivery.` When customers receive new updates regularly, they're more likely to see the changes they want within the product. This leads to happier, more satisfied customers—and more recurring revenue.
- `Welcome changing requirements, even late in the project.` The Agile framework is all about adaptability. In iterative approaches like Agile, being inflexible causes more harm than good. 
- `Deliver value frequently.` Similar to principle #1, continuous delivery of value to your customers or stakeholders frequently makes it less likely for them to churn. 
- `Break the silos of your projects.` Cross-functional teams and collaboration is a key Agile value. The goal is for people to break out of their individual projects and collaborate more frequently. 
- `Build projects around motivated individuals.` Agile management works best when teams are committed and actively working to achieve a goal. 
- `The most effective way to communicate is face-to-face.` If you’re working on a distributed team, spend time communicating in ways that involve face-to-face communication like Zoom calls or daily stand-up meetings. 
- `Working software is the primary measure of progress.` The ultimate goal of software development projects is a working product, and the Agile framework supports this by prioritizing functional software above all.
- `Maintain a sustainable working pace.` Some aspects of Agile project management can be fast-paced, but it shouldn't be so fast that team members burn out. The goal is to maintain sustainability throughout the development process.
- `Continuous excellence enhances agility.` If the team develops excellent code in one sprint, they can continue to build off of it the next. Continually creating great work allows teams to move faster in the future. 
- `Simplicity is essential.` Sometimes the simplest solution is the best solution. Agile development aims to not over complicate things and find simple answers to complex problems. 
- `Self-organizing teams generate the most value.` Similar to principle #5, proactive teams become valuable assets to the company as they strive to deliver continuous improvement.
- `Regularly reflect and adjust your way of work to improve effectiveness.` Retrospective meetings are a common Agile practice. It's a dedicated time for Agile teams to look back and reflect on their performance and adapt their behaviors for the future.

##### Agile Methodologies
There are several frameworks and methodologies under Agile, including:
- `Scrum` - It's a common Agile methodology for small teams and also involves sprints. The team is led by a Scrum master whose main job is to clear all obstacles for others executing the day-to-day work. 
- `Kanban` - It's a visual approach to Agile. Teams use online Kanban board tools to represent where certain tasks are in the development process. Tasks are represented by cards on a board, and stages are represented in columns.
- `Extreme Programming (XP)` - Typically used in software development, Extreme Programming (XP) is an Agile framework that outlines values that will allow your team to work together more effectively.  
- `Lean` - It's  is a way of optimizing organizational processes to maximize customer value while minimizing waste and resources. It emphasizes continuous improvement and the efficient use of resources to streamline processes, reduce costs, and increase quality.
- `Adaptive Project Framework (APF)`- It's also known as Adaptive Project Management (APM) grew from the idea that unknown factors can show up at any time during a project. 
- `Feature-Driven Development (FDD)` - Feature Driven Development blends different Agile best practices. While still an iterative method of project management, this model focuses more on the exact features of a software that the team is working to develop.
- `Dynamic Systems Development Method (DSDM)` - It's is an Agile method that focuses on a full project lifecycle. Because of this, DSDM has a more rigorous structure and foundation, unlike other Agile methods. 
- `Extreme Project Management (XPM)` - This type of project management is often used for very complex projects with a high level of uncertainty. This approach involves constantly adapting processes until they lead to the desired result.

### Scrum Cheat Sheet
#### Scrum
Scrum is an Agile framework where work is delivered in short, time-boxed iterations and Sprints. Each Sprint delivers a potentially shippable product increment, allowing teams to adapt to changing requirements and continuously improve. The Agile process generally follows a cyclical flow where the team iterates through the same process repeatedly to improve and deliver value.

![Agile Process Flow/Workflow](/img/agile-framework.jpg)

#### Agile Process Flow/Workflow
- `Backlog:` This is a list of tasks and user stories that need to be completed.
- `Sprint Planning:` The team picks which user stories to work on for the upcoming sprint.
- `Daily Standups:` A short meeting to discuss progress, challenges, and plans for the day.
- `Sprint Review:` At the end of a sprint, the team demonstrates the work completed.
- `Sprint Retrospective:` The team reviews what went well, what didn’t, and how to improve.

#### Tools for Agile
Some of the tools commonly used to manage Agile projects include:
- Jira
- Trello
- Asana
- Monday.com
- VersionOne
- ClickUp

#### 👥 ROLES IN SCRUM
##### Product Owner (PO)
- Represents the voice of the customer.  
- Manages and prioritizes the Product Backlog.  
- Ensures the team builds the right product.  
- **Core Responsibility:** Communication and Value Maximization  

##### Scrum Master (SM)
- Servant-leader and facilitator for the team.  
- Ensures Scrum principles are followed.  
- Removes impediments and shields the team from distractions.  
- **Core Responsibility:** Scrum implementation and process improvement  

##### The Team (DevOps/Development/DBA/QAE)
- Self-organizing, cross-functional group (3–9 members).  
- Responsible for delivering potentially shippable increments every Sprint.  
- **Core Responsibility:** Delivering high-quality work  

#### ⏱️ ITERATIONS (SPRINTS)
- Sprints are time-boxed iterations where a fixed scope of work is executed.  
- **Typical Length:** 1–4 weeks  
- Once a Sprint starts, the scope is **locked**; new tasks cannot be added.  
- **Outcome:** A working product increment that could be released.

#### 📏 ESTIMATION
Estimation helps teams plan and forecast future work.  
Can be done in:
- **Hours** – Used for precise task duration  
- **Story Points** – Abstract measure based on complexity, risk, and effort  
*Done during backlog refinement or Sprint Planning*

#### 🧱 SCOPE LIMITS
- The Sprint scope is limited to the team’s capacity.  
- Over committing or introducing new work mid-Sprint is discouraged.  
- Focus is on maintaining sustainable pace and delivery quality.

#### 🧩 SCRUM EVENTS / MEETINGS

##### Sprint Planning
- Held at the start of a Sprint (usually 1–2 hours per week of Sprint length).  
- The team and PO agree on the Sprint Goal and the work needed to achieve it.

##### Daily Scrum (Stand-up)
- 15-minute daily sync to inspect progress and adapt the plan.  
- Team members answer:  
  - What did I do yesterday?  
  - What will I do today?  
  - Are there any impediments?

##### Sprint Review
- Held at the end of the Sprint.  
- The team demos the increment to stakeholders and collects feedback.  
- Helps guide future backlog items.

##### Sprint Retrospective
- Held after the Sprint Review and before the next Sprint Planning.  
- Focuses on **process improvement**.  
- Discusses:  
  - What went well?  
  - What didn’t?  
  - What can be improved?

#### 📌 PRIORITIZATION
Managed by the **Product Owner**.  
Items in the Product Backlog are ordered based on:
- Customer value  
- Risk/complexity  
- Dependencies  
- Time sensitivity  
*Helps the team stay focused on high-impact work.*

#### 📋 BOARD (TASK TRACKING)
A typical Scrum board has four key sections:
1. **Product Backlog** – All features, fixes, and requirements (not yet selected for Sprint).  
2. **Sprint Backlog** – Work selected for the current Sprint.  
3. **Doing** – Tasks currently in progress.  
4. **Done** – Completed tasks or stories.  

Boards can be:
- Physical (whiteboards with sticky notes)  
- Digital (e.g., Jira, Trello, Azure Boards)

#### 📘 KEY SCRUM TERMS

##### Product Backlog
A prioritized list of features, enhancements, and bug fixes maintained by the PO.

##### Sprint Backlog
A subset of the Product Backlog selected for a Sprint, broken into tasks by the team.

##### Story Point
A relative unit for estimating effort, used instead of hours to avoid bias and promote velocity tracking.

##### User Story
A short description of functionality from the user's perspective:  
*"As a [user], I want [feature], so that [benefit]."*

##### Burndown Chart
A visual tool showing remaining work in the Sprint over time.  
Helps track progress and identify bottlenecks.

##### Team Velocity
The average number of story points a team can complete in a Sprint.  
Useful for forecasting future Sprints.


#### Comparison between DevOps and Agile in terms of their key aspects:

![Comparison between DevOps and Agile](/img/devops-agile.png)

#### [SDLC (Software Development Lifecycle)](https://aws.amazon.com/what-is/sdlc/)
The software development lifecycle (SDLC) is the cost-effective and time-efficient process that development teams use to design and build high-quality software. The goal of SDLC is to minimize project risks through forward planning so that software meets customer expectations during production and beyond. This methodology outlines a series of steps that divide the software development process into tasks you can assign, complete, and measure.

![Software Development Lifecycle](/img/sdlc.png)

##### SDLC important?
Software development can be challenging to manage due to changing requirements, technology upgrades, and cross-functional collaboration. The software development lifecycle (SDLC) methodology provides a systematic management framework with specific deliverables at every stage of the software development process. As a result, all stakeholders agree on software development goals and requirements upfront and also have a plan to achieve those goals.

**Here are some benefits of SDLC:**
- Increased visibility of the development process for all stakeholders involved
- Efficient estimation, planning, and scheduling
- Improved risk management and cost estimation
- Systematic software delivery and better customer satisfaction

##### How does SDLC work?
The software development lifecycle (SDLC) outlines several tasks required to build a software application. The development process goes through several stages as developers add new features and fix bugs in the software. The details of the SDLC process vary for different teams. However, we outline some common SDLC phases below.
1. `Plan`- Establish project goals, conduct cost-benefit analysis, and gather requirements from stakeholders. Create a Software Requirements Specification (SRS) document to guide the project.
2. `Design`- Analyze requirements and decide on technology, architecture, and integration with existing systems. Plan the system’s structure and user interface.
3. `Implement`- Develop the software by coding it in incremental tasks. Use version control and perform code reviews to ensure quality.
4. `Test`- Conduct automated and manual tests to identify bugs and ensure the software meets the requirements. Testing often overlaps with development.
5. `Deploy`- Move the software from a test environment to production, ensuring a smooth transition without disrupting user access.
6. `Maintain`- Fix bugs, update software, and monitor performance to ensure ongoing stability, security, and user satisfaction.

##### What are SDLC models?
A software development lifecycle (SDLC) model conceptually presents SDLC in an organized fashion to help organizations implement it. Different models arrange the SDLC phases in varying chronological order to optimize the development cycle. We look at some popular SDLC models below.

1. Waterfall
The waterfall model arranges all the phases sequentially so that each new phase depends on the outcome of the previous phase. Conceptually, the design flows from one phase down to the next, like that of a waterfall.

| **Pros**                                          | **Cons**                                                                                          |
| ------------------------------------------------- | ------------------------------------------------------------------------------------------------- |
| Provides discipline to project management.        | Little room for changes once a phase is complete.                                                 |
| Tangible output at the end of each phase.         | Changes can affect delivery time, cost, and quality.                                              |
| Suitable for small software development projects. | Not flexible for larger, more complex projects with evolving requirements.                        |
| Tasks are easy to arrange and manage.             | Requires accurate pre-definition of requirements, which can be difficult in dynamic environments. |

2. Iterative
The iterative process suggests that teams begin software development with a small subset of requirements. Then, they iteratively enhance versions over time until the complete software is ready for production. The team produces a new software version at the end of each iteration.

| **Pros**                                    | **Cons**                                     |
| ------------------------------------------- | -------------------------------------------- |
| Easy to identify and manage risks.          | Repeated cycles could lead to scope changes. |
| Requirements can change between iterations. | Can result in underestimation of resources.  |

3. Spiral
The spiral model combines the iterative model's small repeated cycles with the waterfall model's linear sequential flow to prioritize risk analysis. You can use the spiral model to ensure software's gradual release and improvement by building prototypes at each phase.

| **Pros**                                                | **Cons**                                                    |
| ------------------------------------------------------- | ----------------------------------------------------------- |
| Suitable for large and complex projects.                | Can be expensive for smaller projects with a limited scope. |
| Well-suited for projects that require frequent changes. |                                                             |

4. Agile
The agile model arranges the SDLC phases into several development cycles. The team iterates through the phases rapidly, delivering only small, incremental software changes in each cycle. They continuously evaluate requirements, plans, and results so that they can respond quickly to change. The agile model is both iterative and incremental, making it more efficient than other process models.

| **Pros**                                                         | **Cons**                                                                 |
| ---------------------------------------------------------------- | ------------------------------------------------------------------------ |
| Rapid development cycles help identify and address issues early. | Overreliance on customer feedback could lead to excessive scope changes. |
| Allows engagement with customers and stakeholders for feedback.  | Could result in the project being ended midway or altered excessively.   |

##### [Continuos Integration/Continuos Development (CI/CD)](https://docs.aws.amazon.com/whitepapers/latest/cicd_for_5g_networks_on_aws/cicd-on-aws.html)
It's a software development practice aimed at improving the quality and speed of software delivery. CI/CD pipelines are often implemented using various tools and technologies such as Jenkins, GitLab CI/CD, Travis CI, CircleCI, and others. These tools automate the stages of building, testing, and deployment, enabling development teams to release software more frequently, reliably, and efficiently. We could complete the CI/CD in seven steps (technology stack).

|  SL   | Title             | Activities                                                                                               |
| :---: | :---------------- | :------------------------------------------------------------------------------------------------------- |
|   1   | AWS CodeCommit    | Storing source code (AWS CodeCommit, GitHub, BitBucket etc.).                                            |
|   2   | AWS CodePipeline  | Automating pipeline from source code to Elastic Beanstalk & others (Orchestrate Using From Here).        |
|   3   | AWS CodeBuild     | Building & testing source code (AWS CodeBuild, Jenkins etc.).                                            |
|   4   | AWS CodeDeploy    | Deploying source code (AWS CodeDeploy, Beanstalk, EC2 Instance, On-Premises Instance, Lambda, ECS etc.). |
|   5   | AWS CodeStar      | Manage software development activities such as quick develop, build & deploy, in one place               |
|   6   | AWS Code Artifact | Store, publish, and share software packages to the end point.                                            |
|   7   | AWS CodeGuru      | Automated code reviews using Machine Learning                                                            |

#### Monitoring Tools (Events, Webhooks & Polling)
- Events: 
  You can monitor CodePipeline events in EventBridge, which delivers a stream of real-time data from your own applications, software-as-a-service (SaaS) applications, and AWS services. EventBridge routes that data to targets such as AWS Lambda and Amazon Simple Notification Service. These events are the same as those that appear in Amazon CloudWatch Events, which delivers a near real-time stream of system events that describe changes in AWS resources.
   - Event Pattern
     Each rule is expressed as an event pattern with the source and type of events to monitor, and event targets. To monitor events, you create a rule with the service you are monitoring as the event source, such as CodePipeline. For example, you can create a rule with an event pattern that uses CodePipeline as an event source to trigger the rule when there are changes in the state of a pipeline, stage, or action.
   - Targets
     The new rule receives a selected service as the event target. You might want to set up a target service to send notifications, capture state information, take corrective action, initiate events, or take other actions. When you add your target, you must also grant permissions to EventBridge to allow it to invoke the selected target service.
- Polling:
 It is when your application periodically requests updates from the server. Polling is a simple way to receive updates from a remote server. Your application sends a request to the server at regular intervals, and the server will respond with any updates that have occurred since the last request. Polling is easy to implement and can be a good choice for applications that don't need to receive updates very frequently. However, polling can be inefficient if your application needs to receive updates very quickly, or if the server is slow to respond.

  ![Polling](/img/polling.jpg)
  
- Webhooks:
  Webhooks are when the server sends updates to your application as they happen. Webhooks are a more efficient way to receive updates from a remote server. When you register a webhook with a server, the server will send an HTTP POST request to your application's URL whenever an event occurs. This means that your application will only receive updates when they happen, which can save bandwidth and improve performance. Webhooks are more complex to implement than polling, but they are a good choice for applications that need to receive updates very quickly, or if the server is slow to respond.

  ![Webhooks](/img/webhooks.jpg)

***NB:*** Events are the default & recommended.

#### [Learning Bash Script](https://github.com/jakir-ruet/bashscript-learning)

## With Regards, `Jakir`

[![LinkedIn][linkedin-shield-jakir]][linkedin-url-jakir]
[![Facebook-Page][facebook-shield-jakir]][facebook-url-jakir]
[![Youtube][youtube-shield-jakir]][youtube-url-jakir]

### Wishing you a wonderful day! Keep in touch.

<!-- Personal profile -->

[linkedin-shield-jakir]: https://img.shields.io/badge/linkedin-%230077B5.svg?style=for-the-badge&logo=linkedin&logoColor=white
[linkedin-url-jakir]: https://www.linkedin.com/in/jakir-ruet/
[facebook-shield-jakir]: https://img.shields.io/badge/Facebook-%231877F2.svg?style=for-the-badge&logo=Facebook&logoColor=white
[facebook-url-jakir]: https://www.facebook.com/jakir.ruet/
[youtube-shield-jakir]: https://img.shields.io/badge/YouTube-%23FF0000.svg?style=for-the-badge&logo=YouTube&logoColor=white
[youtube-url-jakir]: https://www.youtube.com/@mjakaria-ruet/featured
