# Describe cloud models

- The cloud models define the deployment types of cloud resources. 
- The three main types of cloud models:
    
    1. Private
    2. Public
    3. Hybrid

### 1. Private Cloud

- The natural evolution from a corporate datacenter.
- It’s a cloud (delivering IT services over the internet) that’s used by a single entity.
- It provides much greater control for the company and its IT department.
- It also comes with greater cost and fewer of the benefits of a public cloud deployment.
- A private cloud may be hosted 
    1. from your on site datacenter.
    2. from a dedicated datacenter offsite.
    3. potentially even by a third party that has dedicated that datacenter to your company.
- Examples:
    1. VMware vSphere
    2. OpenStack
    3. Microsoft Azure Stack
    4. Red Hat OpenShift
    5. HPE GreenLake
    6. IBM Cloud Private
    7. Delll EMC VxRail

### 2. Public Cloud

- It built, controlled, and maintained by a third-party cloud provider.
- Anyone that wants to purchase cloud services can access and use resources. 
- The general public availability is a key difference between public and private clouds.
- Examples: 
    1. Amazon Web Services (AWS)
    2. Microsoft Azure
    3. Google Cloud Platform (GCP)
    4. IBM Cloud
    5. Oracle Cloud infrastructure (OCI)
    6. Alibaba Cloud
    7. Salesforce
    8. Digital Ocean
    9. Rackspace
    10. Tencent Cloud

### 3. Hybrid cloud

- It is a computing environment that uses both public and private clouds in an inter-connected environment. 
- A hybrid cloud environment can be used to allow a private cloud to surge for increased, temporary demand by deploying public cloud resources.
- It can be used to provide an extra layer of security. For example, uses can flexibly choose which services to keep in public cloud and which to deploy to their private cloud infrastructure.
- Examples:
    1. Microsoft Azure Stack
    2. AWS Outposts
    3. Google Anthos
    4. IBM Cloud Satellite
    5. VMware Cloud on AWS
    6. Red Hat OpenShift
    7. Dell Technologies Cloud
    8. HPE GreenLake
    9. Cisco Hybrid Cloud Platform
    10. Oracle Cloud infrastructure (OCI) with Oracle Exadata Cloud at Customer


### Comparing Public, Private and Hybrid Cloud

| Public Cloud | Private Cloud | Hybrid Cloud |
| ------------ | ------------- | ------------- |
| No capital expenditures to scale up | Organizations have complete control over resources and security | Provides the most flexibility |
| Applications can be quickly provisioned and deprovisioned | Data is not collocated with other organizations’ data | Organizations determine where to run their applications |
| Organizations pay only for what they use | Hardware must be purchased for startup and maintenance	| Organizations control security, compliance, or legal requirements |
| Organizations don’t have complete control over resources and security	| Organizations are responsible for hardware maintenance and updates | |


### Multi-cloud

- In this scenario, you use multiple public cloud provides.
- Maybe you use different features from different cloud providers. Or maybe you started your cloud journey with one provider and are in the process of migrating to a different provider.
- Regardless of scenario, in multi-cloud environement you deal with two (or more) public cloud providers and manage resources and security in both environments.

### Azure Arc

- It is a set of technologies that helps manage you cloud environments.
- It can help manage your cloud environmen, whether 
    - it's a public cloud solely
    - a private cloud in your datacenter
    - a hybrid configuration
    - or even a multi-cloud environment running on multiple cloud providers at once.

### Azure VMware Solution

What if you’re already established with VMware in a private cloud environment but want to migrate to a public or hybrid cloud? Azure VMware Solution lets you run your VMware workloads in Azure with seamless integration and scalability.

[Describe the consumption-based model](106-describe-the-consumption-based-model.md)