# Part 1: Linux File System Hierarchy
- / (root) --> Root(top-level directory), all directories and files starts from here.
- /home --> Home directory while accessing user related files or checking user specific info. example: ubuntu
- /root --> Working as root or troubleshooting admin-level issues.
- /etc --> Modifying system or service configurations
- /var/log --> App or log files used for troubleshooting errors identified from logs
- /tmp --> temporary file created which gets cleared on reboot, for test purpose.
- /bin --> Important system command binaries used for running basic commands required for system operation. Ex: ls,cp,mv
- /usr/bin --> User command binaries for running user applications and tools. Ex: Halt, git, stop, start, curl
- /opt --> Optional/third party for installing or managing third party applications.
  <img width="500" height="503" alt="image" src="https://github.com/user-attachments/assets/84ad5ea2-6cec-4b31-aef6-bc765add497f" />
<img width="616" height="284" alt="image" src="https://github.com/user-attachments/assets/e9118498-5aa0-493b-9a41-ae5bd03e556f" />

# Part 2: Scenario Based Questions
## Scenario 1:
- Step 1: sudo systemct status myapp, Why: To check the status of the app service
- Step 2: journalctl -u myapp, Why: To check the service logs if any issues
- Step 3: sudo systemctl is-enabled myapp, Why: To check if myapp service is enabled

## Scenario 2:
- Step 1: top/ htop , Why> To check the live CPU% processes
- Step 2: ps aux --sort=%cpu | head -10, Why> To check the first 10 cpu% processes

## Scenario 3:
- Step 1: systemctl status docker , Why> To check the status of docker
- Step 2: journalctl -u docker -n 50
- Step 3: journalctl -u docker -f, Why> To follow files in real time

## Scenario 4:
- Step 1: ls -l /home/user/backup.sh, Why> To check if backup.sh has execute permission
- Step 2: chmod +x /home/user/backup.sh, Why> To add execute permission
- Step 3: ls -l /home/user/backup.sh, Why> To verify if it worked
- Step 4: ./backup.sh, Why> To run it



