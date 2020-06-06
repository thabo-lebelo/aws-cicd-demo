# aws-cicd-demo

CodeDeploy agent needs to be installed on the instances for CodeDeploy to detect the instances:

#!/bin/bash
yum -y update
yum install -y ruby
cd /home/ec2-user
curl -O https://aws-codedeploy-us-east-1.s3.amazon.com/latest/install
chmod +x ./install
./install auto
