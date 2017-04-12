## Gerard's notes

### Google Cloud Architect study notes

These are the notes I took while studying for the Google Cloud Architect cert. 
I have some experience with GCP as well as AWS and Apache CloudStack so some basic stuff might not be in here.

Start at <https://cloud.google.com/certification/cloud-architect>

It lists the following goals:
> - Design and plan a cloud solution architecture
> - Manage and provision the cloud solution infrastructure
> - Design for security and compliance
> - Analyze and optimize technical and business processes
> - Manage implementations of cloud architecture
> - Ensure solution and operations reliability

There are only two example questions at <https://cloud.google.com/certification/sample#0> so that will not help much.

The exam guide is much more compete: <https://cloud.google.com/certification/guides/cloud-architect/>
The guide is quoted below and my notes are inline.

#### Section 1: Designing and planning a cloud solution architecture

> ##### 1.1	Designing a solution infrastructure that meets business requirements. Considerations include:

> business use cases and product strategy    

> cost optimization    
Google Cloud Platform, GCP, has some mechanisms that can make the monthly bill much lower: autoscaling, appengine vs running VMs, pre-emptible instances. It all starts with the high level design though: what do you really need vs what some (early) requirements say you need.

> supporting the application design    
You can lift&shift a lot of applications to VMs in GCP. To get to big benefits rethink the app design with GCP building blocks in mind. ie. GCP data stores vs running your own DBMS.     

> integration    

> movement of data    
Moving data within GCP is fast and free to cheap, moving in and out of GCP can get slow and pricy. Keep this in mind when making design choices    

> tradeoffs    

> build, buy or modify    

> success measurements (e.g., Key Performance Indicators (KPI), Return on Investment (ROI), metrics)    

> ##### 1.2	Designing a solution infrastructure that meets technical requirements. Considerations include:

> high availability and failover design    
GCP components tend to be fairly well run but to get above 99.9 add redundancy with instance groups, multi-region designs, graceful failures, retries & back-offs & failovers, etc. etc. GCP data stores have settings for redundancy & backups    
> elasticity of cloud resources    

> scalability to meet growth requirements

> ##### 1.3	Designing network, storage, and compute resources. Considerations include:

> integration with on premises/multi-cloud environments

> identification of data storage needs and mapping to storage systems

> data flow diagrams

> storage system structure (e.g., Object, File, RBDMS, NoSQL, New SQL)

> mapping compute needs to platform products

> ##### 1.4	Creating a migration plan (i.e., documents and architectural diagrams). Considerations include:

> integrating solution with existing systems

> migrating systems and data to support the solution

> licensing mapping

> network and management planning

> testing and proof-of-concept

> ##### 1.5	Envisioning future solution improvements. Considerations include:

> cloud and technology improvements

> business needs evolution

> evangelism and advocacy

> #### 2
