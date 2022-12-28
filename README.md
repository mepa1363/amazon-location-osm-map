# Build interactive maps with OpenStreetMap data on AWS

Build a simple web map with the new Open Data Maps option from Amazon Location Service.

## Requirements

To run this project, you will need access to an AWS account with sufficient permissions to create AWS resources. [Create an AWS account](https://portal.aws.amazon.com/billing/signup?trk=15e85350-e523-45c8-9d71-2f9249a4f19f&sc_channel=el), if you do not have one already.

## Create AWS resources

Click the CloudFormation launch stack button to create the necessary AWS resources for this project. The resource include an Amazon Location Service’s map resource, an Amazon Cognito Identity Pool, plus an IAM role and policy.

[![Launch Stack](./cloudformation/launch-stack.svg)](https://console.aws.amazon.com/cloudformation/home?region=us-west-2#/stacks/quickcreate?stackName=open-data-maps-demo&templateURL=https://amazon-location-blog-assets.s3.us-west-2.amazonaws.com/amazon-location-open-data-launch/template.yml)

## Configure

Once the deployment process is complete, go to the CloudFormation console and get the Identity Pool ID from the _Outputs_ section.

Open `index.html` and enter your Cognito Identity Pool ID.

## Run

Open `index.html` in your browser.

## Clean up

To remove the AWS resources created in this project, delete the CloudFormation stack called `open-data-maps-demo`.

Read more about this project [here]().
