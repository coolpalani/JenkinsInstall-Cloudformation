
# Jenkins Installation on EC2 Instance
  This is  a brief notes to installing Jenkins on AWS EC2 instance
## Prerequisites
    AWS account
    AWS CLI installed on the machine
 
  ## Description
   In this repository , we have two templates (yaml files) below. 
  1. Network_Stack
 2. Application_Stack

Network stack accepts  a parameter VPCCIDR  which accepts the CIDR block as input.  
VPC is created in the region the AWS CLI is configured to.

Network created consists of
 - Internet Gateway
 - Route Table with route to Internet Gateway
 - Public subnet with route table above attached

Output from this stack are 
 1. PublicSubnet    
 2.  StackVPC  
 3. MyJenkinsSG

    
  


