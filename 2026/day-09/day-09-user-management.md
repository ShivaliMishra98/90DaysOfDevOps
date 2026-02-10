# Users Created:
- tokyo
- berlin
- professor
- nairobi
# Groups Created:
- developers
- admins
- project-team
# Group Assignment:
- tokyo --> developers
- berlin --> developers and admins
- professor --> admins
- nairobi --> project-team
# Directories Created:
- /opt/dev-project (755)
- /opt/team-workspace (755)
# Commands Used:
- sudo useradd -m tokyo
- sudo useradd -m berlin
- sudo useradd -m professor
- sudo useradd -m nairobi
  ##
- sudo groupadd developers
- sudo groupadd admins
- sudo groupadd project-team
  ##
- sudo gpasswd -a tokyo developers
- sudo gpasswd -a berlin developers // sudo gpasswd -a berlin admins
- sudo gpasswd -a professor admins
- sudo gpasswd -a nairobi project-team
  ##
- sudo mkdir -p /opt/dev-project
- sudo mkdir -p /opt/team-workspace
  ##
- sudo chown root:developers /opt/dev-project
- sudo chmod 2775 /opt/dev-project
- ls -ld /opt/dev-project
- su tokyo
- touch /opt/dev-project/tokyo-text.txt
- exit
- ls -l /opt/dev-project
  ##
  # Learnings:
  - I learnt to create users, add them to group, assign ownership and permissions, setgid bits(s) and how it's needed while changing the owenership of the group
  
