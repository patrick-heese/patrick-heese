# Patrick Heese  

Hi, I’m Patrick.  

I’m an AWS-focused Cloud Administrator moving into Cloud Engineer / Architect roles.  

My portfolio focuses on Infrastructure as Code (IaC), production-style architectures, and clean diagrams and documentation.  

## How I Build  

- **IaC first** - Core infrastructure is provisioned with CloudFormation, SAM, or Terraform with format/lint/plan/change sets. I only use the console where a service really requires it.  
- **IaC quality gate** - Pinned repos call a reusable IaC GitHub Actions workflow that runs formatting, validation, and (optionally) plans or change sets using OIDC to scoped IAM roles.  
- **Security and operations** - Least-privilege IAM, private networking by default, tagging, logs, metrics, alarms.  
- **Consistency** - README structure, architecture diagrams, and verified commits.  
- **Original work** - All Infrastructure as Code, documentation, and diagrams are created by me unless clearly credited in an Acknowledgments section. Some Lambda functions and website components came from course examples; when that happens, I call it out in Acknowledgments.  

---

## Pinned Highlights  

**Cloud Resume Challenge** - Global HTTPS resume on CloudFront + API/DynamoDB; signals: IaC, OIDC CI/CD, least-privilege IAM.  
Services: CloudFront, API Gateway, Lambda, DynamoDB · IaC: Terraform  
[aws-cloud-resume-challenge](https://github.com/patrick-heese/aws-cloud-resume-challenge)  

![IaC Gate](https://github.com/patrick-heese/aws-cloud-resume-challenge/actions/workflows/infra-ci.yml/badge.svg)  

**Site-to-Site VPN (TGW + BGP)** - Dual-tunnel IPsec to TGW with BGP propagation; signals: failover tested, private-only workloads.  
Services: VPC, Transit Gateway, VPN/IPsec, EC2 · IaC: CloudFormation  
[aws-tgw-site-to-site-vpn](https://github.com/patrick-heese/aws-tgw-site-to-site-vpn)  

![IaC Gate](https://github.com/patrick-heese/aws-tgw-site-to-site-vpn/actions/workflows/infra-ci.yml/badge.svg)  

**Secure Application on AWS (Security Pillar)** - ALB→EC2/RDS in private subnets with WAF + managed rules; signals: least-privilege IAM, encrypted at rest/in transit.  
Services: ALB, EC2, RDS, WAF, S3 · IaC: CloudFormation  
[aws-securecart-security-pillar](https://github.com/patrick-heese/aws-securecart-security-pillar)  

![IaC Gate](https://github.com/patrick-heese/aws-securecart-security-pillar/actions/workflows/infra-ci.yml/badge.svg)  

**3-Tier WordPress Website on AWS** - ALB → EC2 + EFS + RDS (Multi-AZ); signals: IaC, SSM-sourced secrets, no public DB access.  
Services: VPC, ALB, EC2 ASG, RDS Multi-AZ, EFS · IaC: CloudFormation  
[aws-wordpress-three-tier-website](https://github.com/patrick-heese/aws-wordpress-three-tier-website)  

![IaC Gate](https://github.com/patrick-heese/aws-wordpress-three-tier-website/actions/workflows/infra-ci.yml/badge.svg)  

**Stock Market Analytics Pipeline** - Streaming data pipeline (Kinesis → Lambda → Athena); signals: at-least-once delivery, idempotent processing, IaC, OIDC CI/CD.  
Services: Kinesis, Lambda, DynamoDB, S3, Athena, SNS · IaC: SAM  
[aws-stock-market-analytics-pipeline](https://github.com/patrick-heese/aws-stock-market-analytics-pipeline)  

![IaC Gate](https://github.com/patrick-heese/aws-stock-market-analytics-pipeline/actions/workflows/infra-ci.yml/badge.svg)  

**2048 CI/CD (ECS/ECR)** - Automated build/test/deploy to ECS Fargate; signals: zero-secrets OIDC, gated deploys via CodePipeline/CodeBuild.  
Services: ECR, ECS Fargate, CodePipeline, CodeBuild, CloudWatch Logs · IaC: Terraform  
[aws-2048-game-cicd-pipeline](https://github.com/patrick-heese/aws-2048-game-cicd-pipeline)  

![IaC Gate](https://github.com/patrick-heese/aws-2048-game-cicd-pipeline/actions/workflows/infra-ci.yml/badge.svg)  

---

## Project Catalog  

<details open>
<summary><strong>Applications & Serverless</strong></summary>  

- Serverless Inventory Management (Performance Efficiency Pillar)  
  Services: Amplify, API Gateway, Lambda, DynamoDB, CloudWatch · IaC: SAM  
  [aws-coffeeshop-manager-performance-efficiency-pillar](https://github.com/patrick-heese/aws-coffeeshop-manager-performance-efficiency-pillar)  

- Serverless Cloud Dictionary  
  Services: Amplify, API Gateway, Lambda, DynamoDB · IaC: Terraform  
  [aws-serverless-cloud-dictionary](https://github.com/patrick-heese/aws-serverless-cloud-dictionary)  

- Event Announcement System  
  Services: SNS, Lambda, API Gateway, S3, IAM · IaC: SAM  
  [aws-event-announcement-website](https://github.com/patrick-heese/aws-event-announcement-website)  

- Bucket List Tracker Application  
  Services: Amplify, AppSync (GraphQL), DynamoDB, S3 · IaC: N/A  
  [aws-bucket-list-tracker](https://github.com/patrick-heese/aws-bucket-list-tracker)  

</details>  

<details open>  
<summary><strong>Web, Containers, Multi-Cloud</strong></summary>  

- Highly Available Architecture (Reliability Pillar)  
  Services: VPC, ALB, EC2 ASG, RDS Multi-AZ, Route 53, S3, EFS · IaC: CloudFormation  
  [aws-medicare-hub-reliability-pillar](https://github.com/patrick-heese/aws-medicare-hub-reliability-pillar)  

- Two-Tier Website on AWS  
  Services: EC2, RDS, ALB, VPC · IaC: CloudFormation  
  [aws-to-do-list-two-tier-website](https://github.com/patrick-heese/aws-to-do-list-two-tier-website)  

- Multi-Cloud Weather Tracker (DR)  
  Services: S3, CloudFront (+ Azure Blob failover) · IaC: Terraform  
  [aws-azure-dr-weather-tracker-website](https://github.com/patrick-heese/aws-azure-dr-weather-tracker-website)  

</details>  

<details open>  
<summary><strong>Data & Analytics</strong></summary>  

- Automated Receipt Processing System  
  Services: S3, Textract, DynamoDB, SES, Lambda · IaC: SAM  
  [aws-receipt-processing-system](https://github.com/patrick-heese/aws-receipt-processing-system)  

- Weather Data Processing Pipeline  
  Services: S3, Lambda, Glue, QuickSight, IAM · IaC: Terraform  
  [aws-weather-data-processing-pipeline](https://github.com/patrick-heese/aws-weather-data-processing-pipeline)  

</details>  

<details open>  
<summary><strong>Automation, Cost, and Ops</strong></summary>  

- Automated Cost Governance (Cost Optimization Pillar)  
  Services: S3, EC2, SSM, SNS, Cost Explorer, Trusted Advisor, CloudFormation · IaC: CloudFormation  
  [aws-cost-governance-cost-optimization-pillar](http://github.com/patrick-heese/aws-cost-governance-cost-optimization-pillar)  

- Real-Time AWS Operations from Slack (Operational Excellence)  
  Services: Amazon Q Developer in Slack, CloudWatch, EventBridge, Lambda, SSM, CloudFront, S3 · IaC: CloudFormation  
  [aws-chatops-operational-excellence-pillar](https://github.com/patrick-heese/aws-chatops-operational-excellence-pillar)  

</details>  

<details open>  
<summary><strong>ML / GenAI</strong></summary>  

- Cloud Fun Facts Generator  
  Services: Bedrock, Lambda, API Gateway, DynamoDB, Amplify · IaC: SAM  
  [aws-cloud-fun-facts-generator](https://github.com/patrick-heese/aws-cloud-fun-facts-generator)  

- Image Labels Generator  
  Services: S3, Rekognition · IaC: Terraform  
  [aws-rekognition-image-label-generator](https://github.com/patrick-heese/aws-rekognition-image-label-generator)  

- SageMaker Threat Detection System  
  Services: SageMaker, S3, Lambda, CloudWatch, IAM · IaC: Terraform  
  [aws-sagemaker-threat-detection-system](https://github.com/patrick-heese/aws-sagemaker-threat-detection-system)  

- Daily Task Scheduler - Built with Amazon PartyRock.  
  Services: PartyRock · IaC: N/A  
  [aws-partyrock-daily-task-scheduler](https://github.com/patrick-heese/aws-partyrock-daily-task-scheduler)  

</details>  

<details open>  
<summary><strong>Chat/Voice/Translation</strong></summary>  

- Lex Language Translation Bot  
  Services: Lex, Lambda, Translate, IAM · IaC: SAM  
  [aws-lex-language-translation-bot](https://github.com/patrick-heese/aws-lex-language-translation-bot)  

- Polly Text Narrator  
  Services: Polly, IAM · IaC: Terraform  
  [aws-polly-text-narrator](https://github.com/patrick-heese/aws-polly-text-narrator)  

</details>  

---

## Contact  

- GitHub: https://github.com/patrick-heese/  
- LinkedIn: https://www.linkedin.com/in/patrick-heese/  
- Email: pheese8@gmail.com  
