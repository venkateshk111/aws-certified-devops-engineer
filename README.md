# aws-certified-devops-engineer
AWS Certified DevOps Engineer Guide


## Lambda
 - Reserved concurrency Vs Provisioned Concurrency ?

    | Feature               | Reserved Concurrency  | Provisioned Concurrency |
    |-----------------------|-----------------------|-------------------------|
    | Description           | Allows setting a concurrency limit for a specific function, ensuring that the specified number of invocations will run concurrently. | Pre-warms a specified number of instances of a function to handle traffic immediately, without cold starts. |
    |     Invocation        | Ensures that only the specified number of invocations of that function can run concurrently, regardless of the overall concurrency limits for the account. | Ensures consistent performance and low latency for functions that require it. |
    |    Use Case        | Useful for controlling the resource usage and performance of critical functions. | Helpful for applications with sudden or high spikes in traffic. |


 - **Lambda function concurrency limit** : This is the overall limit on the number of concurrent executions across all functions in your account. By default, this limit is 1000, but it can be increased by contacting AWS Support.

## Amazon SQS 
 - *`ApproximateAgeOfOldestMessage`*
 - *`NumberOfMessagesSent`*

## AWS DevOps

## CodeCommit


## CodeBuild


## CodeDeploy
 - CodeDeploy Environment Variables
    1. **LIFECYCLE_EVENT** : This variable contains the name of the lifecycle event associated with the script.
    2. **DEPLOYMENT_ID** :  This variables contains the deployment ID of the current deployment.
    3. **APPLICATION_NAME** :  This variable contains the name of the application being deployed. This is the name the user sets in the console or AWS CLI.
    4. **DEPLOYMENT_GROUP_NAME** :  This variable contains the name of the deployment group. A deployment group is a **set of instances associated with an application that you target for a deployment**.
    5. **DEPLOYMENT_GROUP_ID** : This variable contains the ID of the deployment group in AWS CodeDeploy that corresponds to the current deployment

 - AppSpec file ?

## CodePipeline



## AWS Config
 - AWS Config can be used to meet your organization compliance requirements like resource tagging etc etc
 - Use managed rules where ever applicable
 - AWS Config allows you to develop custom rules using AWS Lambda. 
    - Example: You can create a custom rule that checks the last rotation date of each AWS KMS key and publishes a message to an Amazon SNS topic if a key has not been rotated in the last 90 days


## Encryption 

## AWS GuardDuty
 - Amazon GuardDuty is a **threat detection service** that **continuously monitors for malicious activity and unauthorized behavior**

## AWS WAF

## AWS FireWall Manager
 - AWS Firewall Manager allows you to **centrally configure and manage AWS WAF rules across your accounts and applications in AWS Organizations**.