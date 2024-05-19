## [Lessons Learned from the Capital One Data Breach (PDF)](https://www.zscaler.com/resources/white-papers/capital-one-data-breach.pdf)

### What were the three commands used for the attack?
* Get Credentials - When executed obtains security credentials known as a WAF-Role account (an IAM account) for an elevated role access AWS Web Application Firewall (WAF)
* List Buckets - When executed, uses the security credentials WAF-Role account to list files and folders (aka S3 buckets)
* Download Files - When executed use the WAF-Role account to download files accessible by the credentials.
### What misconfiguration of AWS components allowed the attacker to access sensitive data?
At the application layer (layer 7) of a firewall installed by the Financial Institution, they were exacerbated by permissions set by the Financial Institution that were likely broader than intended.
### What are two of the AWS Governance practices that could have prevented such an attack?
Network Segmentation and access controls, and the Principle of Least Privilege are two AWS Governance practices that could have prevented such attacks.
