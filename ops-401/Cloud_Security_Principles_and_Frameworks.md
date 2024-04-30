## [AWS Architecture Blog - Compute Abstractions on AWS: A Visual Story](https://aws.amazon.com/blogs/architecture/compute-abstractions-on-aws-a-visual-story/)
### Explain the levels of abstraction in AWS to someone without a technical background.
* ***Infrastructure as a Service (IaaS):***
  * Imagine buying land: When you buy land, you get an empty plot. You’re responsible for building everything house, road, and utilities. In AWS, this is like renting a virtual server (EC2 instance). You choose the size and type, but you handle the rest like setting up the house (operating system) and utilities (security).
* ***Platform as a Service (PaaS):***
  * Think of renting an apartment: In a apartment, you don’t worry about land or building, it’s all provided. You just focus on decorating your space. In AWS, PaaS services (Amazon RDS for databases) are like fully furnished apartments. AWS manages the infrastructure, backups, and scaling.
* ***Function as a Service (FaaS):***
  * Picture hiring a caterer for a party: You don’t cook, serve, or clean up. The caterer handles it all. Similarly, in AWS, AWS Lambda is like a caterer for code. You write small functions, and Lambda runs them when needed. No server management required!
* ***Software as a Service (SaaS):***
  * Using a microwave: You pop in food, press a button, and enjoy a hot meal. You don’t need to know how the microwave works. In AWS, SaaS services (Amazon S3 for storage) work similarly. You use them without worrying about the underlying details.
### What are the control plane and data plane responsible for in container abstraction?
* Containers control plane is responsible for exposing the API and interfaces to define, deploy, and lifecycle containers. This is also sometimes referred to as the container orchestration layer.
* Containers data plane is responsible for providing capacity (as in CPU/Memory/Network/Storage) so that those containers can actually run and connect to a network. From a practical perspective this is typically a Linux host or less often a Windows host where the containers get started and wired to the network.
### Where does AWS Lambda fall in the layers of abstraction and what makes it so special?
AWS Lambda falls in all the layers of abstraction and what makes it so special its serverless and event-driven

##### ***Bookmark and Review***
##### ***[13 Compliance Frameworks for Cloud-based Orgs](https://www.horangi.com/blog/13-compliance-frameworks-for-cloud-based-organizations)***
##### ***[Cloud Security Alliance](https://cloudsecurityalliance.org/) (CSA)***
  * ##### ***[Cloud Controls Matrix](https://cloudsecurityalliance.org/research/cloud-controls-matrix) (CCM)***
  * ##### ***[CSA Security Guidance for Cloud Computing](https://cloudsecurityalliance.org/research/guidance)***
