## COMMANDS CHEATSHEET 
- ps aux | grep nginx --> Active processes filter specific
- htop --> Real-time process
- kill -9 (PID) --> To kill a process
- systemctl status nginx  --> To check the status of a process (like nginx)
- systemctl start docker  --> To start services
- systemctl enable httpd  --> To start services post reboot
- journalctl -u nginx  --> To check the service logs
  ##
- pwd  --> present working directory
- ls  --> List the files
- cd  --> change directory
- cat file_name  --> To view the contents of a file
- mkdir -p /josh/devops/files  --> To specify the path of creating folder/files
- ls -l   --> It prints the premissions of the folder / files
- sudo chmod 400 new-file.txt  --> Giving Read permission to Owner
- sudo chmod 777 new-file.txt  --> Giving all Read, Write, Executable permissions to Owner, Group, Other users
- sudo chown tokyo josh-batch-10.txt  --> Changing Owner of josh-batch-10.txt file from Ubuntu to Tokyo directory
##
- ping trainwithshubham.com  --> To ping server and check if all packets transmitted and received
- ip addr  --> To show Network Devices/Routing/interfaces/tunnels
- dig  --> DNS Lookup utility
- curl google.com  --> Transfer a URL
