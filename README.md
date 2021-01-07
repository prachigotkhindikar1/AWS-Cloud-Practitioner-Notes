# AWS-Cloud-Practitioner-Notes


### APN Partner Types
* APN Technology partners : Provide customers software solutions that are either hosted on, or integrated with AWS platform. 
* APN Consulting Partners : Professional firms that help customers of all sizes design, architect, build, migrate and manage their workloads and applications on AWS.


### AWS Premium Support Teams
* AWS Security Team : Assist with security of services offered by AWS
* AWS Abuse Team : Assist with reports related to malicious use of AWS resources for abusive or illegal purposes.ex: spam, port scanning, DoS, intrusion attempts, distribute malware.
* AWS Concierge Team : Assist with billing support and account management
* AWS Customer Service team : Assist customers understand the importance of Cloud Computing and how it can be useful to their business needs.


### Code* services

* CodeStar : CodeStar connects CodeCommit/git, CodeBuild, CodePipeline, and CodeDeploy together using predefined templates. It’s just an overlay to the underlying services to simplify the orchestration. If you need to add in additional complexity, such as manual approval gates, then it may be better to use the services directly.
* Codebuild : AWS CodeBuild is a fully managed continuous integration service that compiles source code, runs tests, and produces software packages that are ready to deploy. With CodeBuild, you don’t need to provision, manage, and scale your own build servers. CodeBuild allows you to build applications from code stored in repositories, but CodeBuild itself will not host the code
* CodeCommit : AWS CodeCommit is a fully-managed source control service that hosts secure Git-based repositories. Eliminates the need to manage own Source control and scale it.
* CodeDeploy : Managed deployment service that automates Software deployments to variety of compute services.
* CodePipeline : Fully managed CD service that automates the release process.


### AWS WellArchitected Framework 5 Pillars

* **C** - Cost Optimization
* **O** - Operational Excellence
* **R** - Reliability. (Failure Recovery, Automatic provision of new resources on demand)
* **P** - Performance efficiency
* **S** - Security


### AWS Architecture Best Practices
http://aws001.s3.amazonaws.com/trailhead/TrailHead_ArchitectingInTheCloud.pdf

- Design for failure and nothing else fails
  - Deploy to multiple regions and AZs as needed
  - use of ELB to distribute loads
  - use of auto-scaling
- Loose coupling sets you free
  - Independent components 
  - Design everything as blackbox
  - load balance clusters
  - Use AWS SQS as buffers
- Implement Elasticity
  - Adjusting compute capacity dynamically to reduce cost
- Build security in every layer
- Don't fear constraints
- Think parallel
- Leverage many storage options
  - Amazon S3: large static objects
  - Amazon CloudFront: content distribution
  - Amazon SimpleDB: simple data indexing/querying
  - Amazon EC2 local disc drive : transient data
  - Amazon EBS: persistent storage for any RDBMS + Snapshots on S3
  - Amazon RDS: RDBMS service - Automated and Managed MySQL
