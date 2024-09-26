# Cost-optimization-AWS

Lambda function identifies EBS snapshots that are no longer associated with any active EC2 instance and deletes them to save on storage costs

By default there is volumes attached to EC2 instance and those volumes are filled with the sensitive data of the org, so a backup is needed where a developer takes snapshots

so when the developer forgets to delete snapshots and deletes the ec2/ volume after using it, AWS stills costs for the storage of snapshots (this is not only limited to EC2 service)

we will be using lambda function of python code with module a called boto3 ( for communicating with AWS API) to delete the EBS snapshots

we can also attach this function using cloudwatch 
/*(this code will get an error :
1.edit the time to execute to 10 sec in config tab
2. give permission to IAM roles and create policies for decribe instances, snapshots..... or you can select all permissions(worst case) )*/

![WhatsApp Image 2024-09-27 at 00 19 22_c23bacf8](https://github.com/user-attachments/assets/4905df78-231b-4390-ba9d-46d9f7f99854)

![WhatsApp Image 2024-09-27 at 00 22 21_d1083acb](https://github.com/user-attachments/assets/5b17f4e6-0f37-47aa-940b-dae669ef1bf9)

![WhatsApp Image 2024-09-27 at 00 24 21_719b466a](https://github.com/user-attachments/assets/75b56f46-a2cd-4d3f-8cf6-6f47e915a484)


