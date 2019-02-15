# Overview
In this lab you'll learn how to enable AWS Security Hub as part of a multi-account strategy and how to configure and navigate the service to start getting visibility of security events and compliance across your organisation.

# Inital Setup
<details>
<summary><strong>Deploy infratsructure to fake security events</strong></summary><p>

In order to have some metrics to work with we'll deploy a single EC2 instance with code to generate some fake GuardDuty events. This CloudFormation template will also create a publicably readable S3 bucket.

| AWS Region | Short name | |
| -- | -- | -- |
| EU West (London) | eu-west-2 | <a href="https://console.aws.amazon.com/cloudformation/home?region=eu-west-2#/stacks/new?stackName=fake-insecure-account-details&templateURL=https://s3-eu-west-1.amazonaws.com/aws-shared-demo-cf-templates/insecure-account-for-security-demos/master_template.yaml" target="_blank"><img src="images/cloudformation-launch-stack.png"></a> |

</details>

<details>
<summary><strong>Enable Security Hub</strong></summary><p>

1. From the AWS console search for Security Hub in the search box and select the service.
    <p align="left">
      <img width="400" src="https://github.com/charliejllewellyn/aws-shared-demo-lab-guides/blob/master/security-hub/images/sec-hub-service.png">
    </p>
1. On the right-hand side select **Enable Security Hub**
    <p align="left">
      <img width="400" src="https://github.com/charliejllewellyn/aws-shared-demo-lab-guides/blob/master/security-hub/images/enable-sec-hub.png">
    </p>
1. Click **Enable AWS Security Hub**
</details>

# Configuring basic 
