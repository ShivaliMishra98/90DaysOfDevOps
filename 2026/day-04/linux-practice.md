## INSTALLING DOCKER WORKFLOW
- First, update the packages using <mark>sudo apt update -y</mark> to install Docker
- Now, install Docker using <mark>sudo apt install docker.io</mark>
##
- <mark>ps aux | grep docker</mark>
  >> Lists active process like containerd, root
- <mark>htop</mark>
  >> Lists real-time running processes with CPU and Memory usages too
- <mark>sudo systemctl status docker</mark>
  >> Active (Running) status
- <mark>systemctl list-units</mark>
  >>   -.mount                                                 
  boot-efi.mount                                                           
  boot.mount                                                                   
  dev-hugepages.mount                                                         
  dev-mqueue.mount
##
- <mark>journalctl -u docker</mark>
  >> Feb 07 19:57:47 ip-172-31-16-205 systemd[1]: Starting docker.service - Docker Application Container Engine...
  level=info msg="Daemon h
   Docker Application Container Engine.
- <mark>tail -n 50 /var/log/syslog</mark>
  >> Prints last 50 lines of the logs 
  
