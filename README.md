# UdaApp
Create cloud formation IAC=>Project 2 Cloud DevOps Engineer Udacity

# Steps to deployment
1. Install aws2 cli on your machine
2. Open the terminal
3. Run `aws configure` to configure the IAM profile --region us-east-1
4. Run `cd ./UdaApp`
5. Run `./create.sh --stackname stackname1 udainfra.yml uda-prams.json` to provision the VPC with some resources
6. Wait for the CREATE_COMPLETE status in the aws console
7. Run `./create.sh --stackname stackname2 uda-server.yml uda-server.json` to provision the security groups and loadbalancers with the Launch configs
8. Wait for the CREATE_COMPLETE status for the second stack
9. Check the health of the target groups. If healthy then go to the LB and copy the dns name
10. Done
