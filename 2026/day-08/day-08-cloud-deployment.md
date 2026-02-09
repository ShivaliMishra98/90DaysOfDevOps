# Deploying Cloud Server (nginx)
<img width="598" height="492" alt="image" src="https://github.com/user-attachments/assets/a220d61b-22fb-42b8-804b-cb2853ac3393" />
<img width="959" height="305" alt="image" src="https://github.com/user-attachments/assets/4a7d568f-b68a-46d1-b183-870638ea7a28" />
<img width="959" height="501" alt="image" src="https://github.com/user-attachments/assets/32f04bb1-7c04-4ee0-a7ad-575855403327" />

# Document:
- Key Commands:
  - sudo systemctl install -y nginx
  - sudo syaytemcyl status nginx
  -  scp -i Linux-Key.pem ubuntu@54.224.176.143:~/nginx-logs.txt .
  -  ls nginx-logs.txt
- Challenges faced were while generating the nginx.logs while using the nginx-logs.txt
- We can deploy an app on this service nginx and evn congiure it's security group of the EC2, generate the logs.
