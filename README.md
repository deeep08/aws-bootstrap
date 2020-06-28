# aws-bootstrap
Sample AWS Hello World Application: From <a href="https://www.educative.io/">educative</a> course - 
<a href="https://www.educative.io/collection/10370001/5943367834796032">The Good Parts of AWS: Cutting Through the Clutter</a>

<hr>

This project demonstrates the use of CloudFormation to deploy a simple web application along with all the required AWS resources
<ul>
    <li>VPC</li>
    <li>Internet Gateways</li>
    <li>Public and Private Subnets</li>
    <li>Route Table</li>
    <li>Security Groups</li>
    <li>IAM Role and Instance Profile</li>
    <li>NAT Gateways</li>
    <li>Launch Templates</li>
    <li>Auto Scaling Groups</li>
</ul>

This project creates a CodePipeline to deploy the project onto the Staging and Production environment whenever a commit is made to the project repository.
To achieve this, it also uses AWS CodeBuild and CodeDeploy services.

A simple nodejs http/https server is used as a sample web application in this project to demonstrate the use of 
- CodePipeline
- CodeBuild  
- CodeDeploy

To create all the AWS resources and deploy the sample web application, just run the below command from Project root directory

<code>./deploy-infra.sh</code>

You may need to update the following variables in the script "deploy-infra.sh" to make it work:-

<ul>
    <li>AWS_ACCOUNT_ID</li>
    <li>GH_ACCESS_TOKEN</li>
    <li>GH_OWNER</li>
    <li>GH_REPO</li>
    <li>GH_BRANCH</li>
    <li>STACK_NAME</li>
    <li>REGION</li>
    <li>CLI_PROFILE</li>
    <li>EC2_INSTANCE_TYPE</li>
    <li>DOMAIN</li>
    <li>CERT</li>
    <li>CODEPIPELINE_BUCKET</li>
    <li>CFN_BUCKET</li>
</ul>

The above script print the endpoint using which the site can be opened.