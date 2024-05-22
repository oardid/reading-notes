## [What is Amazon GuardDuty?](https://docs.aws.amazon.com/guardduty/latest/ug/what-is-guardduty.html)

### What are some of the IoCs that GuardDuty can detect?
GuardDuty can detect compromised EC2 instances and container workloads serving malware, or mining bitcoin. 
### What are some of the data sources which GuardDuty can use?
Some of the data sources that GuardDuty can use are AWS CloudTrail management events, AWS CloudTrail event logs, VPC flow logs (from Amazon EC2 instances), and DNS logs.
### How does GuardDuty use access behavior to spot potential malicious activity?
Signs of potential compromise include unauthorized infrastructure deployments, such as instances deployed in a region that hasn't been used before, or unusual API calls, such as changing the password policy to reduce password strength.
