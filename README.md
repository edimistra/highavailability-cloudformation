# highavailability-cloudformation
Deploy a high-availability web app using CloudFormation scripts that includes server and network components

## Files

### 1. Infrastructure diagram
- High Availability Web App.pdf

### 2. CloudFormation files
- network.yml
- network-parameters.json
- servers.yml
- server-parameters.json

### 3. Shell scripts
- create.sh
- update.sh
- create.bat
- update.bat

### 4. URL to validate that the project runs
http://serve-webap-1fp0ogij28q6g-1305853584.us-west-2.elb.amazonaws.com/index.html

### 5. How to run in your cloud
- Make sure to have already intalled AWS CLI
- > ./create.sh <stack name> network.yml network-parameters.json
- > ./create.sh <stack name> servers.yml server-parameters.json
- Go to CloudFormation in the AWS console and get the load balancer DNS name from the output parameters
  
### 6. Important notes:
- Used t2.micro (1 vCPU 1GB RAM) instead of t2.medium (2 vCPU 4GB RAM) since t2.micro is on the Free Tier
