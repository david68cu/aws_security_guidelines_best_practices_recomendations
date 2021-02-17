## AWS Security Infraestructure

- I-   Security Frameworks and  Guidelines(OWASP, NIST, CIS and also AWS Security Best Practice for each service)
- II-  AWS Compliances and Standards for Certification (HIPAA,PCI, FedRAMP)
- III- AWS Native Security Tools
- IV-  AWS DevOps Security  and DevOps Security Pipeline
- V-   AWS CLI 
- VI-  Python tools and development 


### I- Security Frameworks and  Guidelines(OWASP, NIST, CIS)

- OWASP
   - Container Security Verification Standard 
   - (https://github.com/OWASP/Container-Security-Verification-Standard )

- NIST 
  - NIST Special Publication 800-190
  - Application Container Security Guide
  - (https://nvlpubs.nist.gov/nistpubs/specialpublications/nist.sp.800-190.pdf)

- CIS (Center for Information Security)
  - Securing Docker
  - (https://www.cisecurity.org/benchmark/docker/)

- [OWASP AWS documents in Archive](https://owasp.org/www-pdf-archive/)
  - 1- (https://owasp.org/www-pdf-archive//AWS_Security_-_Staying_on_Top_of_the_Cloud.pdf
  - 2- https://owasp.org/www-pdf-archive//Aws_security_joel_leino.pdf
  - 3- https://owasp.org/www-pdf-archive//OWASP_Toronto_-_Aug_2017_-_Cloud_Security_&_Best_Practice_in_AWS_by_Ankit_Giri.pdf

- AWS Security Best Practice(SBP) and Recomendations for each service
  - [Security Best Practices for Amazon S3](https://aws.amazon.com/s3/security/?nc=sn&loc=5)
  - [Security Best Practices for Amazon EC2](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ec2-security.html)
  - [Security Best Practice for Serverless](https://docs.aws.amazon.com/whitepapers/latest/serverless-architectures-lambda/security-best-practices.html)
  - [Security Best Practice for Kubernettes EKS](https://docs.aws.amazon.com/eks/latest/userguide/best-practices-security.html)
  - [Security Best Practice for Kubernettes ECS](https://docs.aws.amazon.com/AmazonECS/latest/developerguide/security.html)

- AWS Whitepapers 
   - A collection of AWS Whitepapers where we can filter for security concersn at https://aws.amazon.com/whitepapers/

- AWS Security Blog
  - AWS Security Blog: https://aws.amazon.com/blogs/security/tag/devsecops/

## II- AWS Compliances and Standards for Certification (HIPAA,PCI, FedRAMP)

 [References](https://aws.amazon.com/compliance/)
 
- 1	The Federal Risk and Authorization Management Program (FedRAMP) is a US government-wide program that delivers a standard approach to the security assessment, authorization, and continuous monitoring for cloud products and services
- 2	FedRAMP documents https://d1.awsstatic.com/whitepapers/compliance/Guidance_for_Trusted_Internet_Connection_TIC_Readiness_on_AWS.pdf
- 3	HIPAA https://aws.amazon.com/compliance/hipaa-compliance/
- 4	PCI https://aws.amazon.com/compliance/pci-dss-level-1-faqs/
- 5	FedRAMP https://aws.amazon.com/compliance/fedramp/

### III- AWS Native Security Tools

-	Each Service has its own security concerns that we should look in AWS documentation.

   -	AWS CloudWatch:   https://aws.amazon.com/cloudwatch/
   -	AWS CloudTrail:   https://aws.amazon.com/cloudtrail/
   -	AWS Config:       https://aws.amazon.com/config/
   -	AWS Inspector:    https://aws.amazon.com/inspector/
   -	AWS Guard Duty:   https://aws.amazon.com/guardduty/
   -	AWS WAF:          https://aws.amazon.com/waf
   -	AWS Shield:       https://aws.amazon.com/shield/
   -	AWS Security Hub: https://aws.amazon.com/security-hub/
   -	AWS Macie:        https://aws.amazon.com/macie/
   -	AWS X-Ray:        https://aws.amazon.com/xray/

### IV- AWS DevOps Security  and DevOps Security Pipeline

Ref: https://github.com/david68cu/aws-architect-project3-Implementing-Security

Four Aspect to take into account for a technician from a practical perspective

- IV.1 AWS DevOps Security Pipeline
- IV.2 Infrastructure as Code Scanning Tools(Terraform and CloudFormation)
- IV.3 Scan containers for OS Vulnerabilities
- IV.4 Qualys Virtual Scanner Appliance HVM 


#### IV.1- AWS DevOps Security Pipeline

![Dev Sec Operations Pipeline](DevSecOpsPipline.png)

#### IV.2 Infrastructure as Code Scanning Tools

- CloudFormation scanning tools Ex: Cfripper. Some of the compliance violation or vulnerability which it might expose.

  - open S3 buckets,
  - unnecessarily wide port ranges on EC2 instances,
  - disabled encryption on databases and more.
  
- Terraform scanning tools Ex: Terrascan( https://github.com/accurics/terrascan)

  - Detect compliance and security violations across Infrastructure as Code to mitigate risk before provisioning cloud native infrastructure.
  - 500+ Policies for security best practices
  - Scanning of Terraform (HCL2)
  - Scanning of Kubernetes (JSON/YAML), Helm v3, and Kustomize v3
  - Support for AWS, Azure, GCP, Kubernetes and GitHub

#### IV.3 Scan containers for OS Vulnerabilities

Chef InSpec: execute scans against local or remote machines .

#### IV.4 Qualys Virtual Scanner Appliance HVM

- Qualys provides a cloud agent that can be installed either on EC2 or at the source into AMI for automated asset discovery ,classification, monitoring, and vulnerability remediation.
  -	What ports are open in an instance?
  - What ports are listening for connections?


## V- AWS CLI 

-	Programmatically accessing multiple aws api to retrieve information about the services they offer
-	Programmatically accessing multiple aws sdk to configure new services

## VI- Python tools, programming and integrations




