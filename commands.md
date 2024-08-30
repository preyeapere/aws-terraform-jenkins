We shall be installing Jenkins software on port 8080
we shall be creating the custom virtual cloud public subnet,private subnet and EC2 Instances all will be done using terraform infrastructure as code.

Authenticate with AWS.
(You must install AWS CLI)

aws configure

aws sts get-caller-identity

aws s3 ls

terraform init

4.0  Run this comand to format all your terraform files

     terraform fmt



5.0  Run this command to viladate your terraform script

     terraform validate



6.0  Run this command to showcase all the recourses you want to create using terraform

     terraform plan

     

7.0  Run this command to apply all you resources and create the all within aws infrastruct

     terraform apply --auto-approve

     
put you public ip 13.60.86.106:8080 on your browser

SSH to your machinessh -i "gold.pem" ubuntu@13.60.86.106

when inside the machine run 
sudo cat /var/lib/jenkins/secrets/initialAdminPassword

Paste the Password into the jenkin browser