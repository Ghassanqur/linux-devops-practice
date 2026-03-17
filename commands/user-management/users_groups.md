# User and Group Management

## Create User
sudo useradd devuser
sudo passwd devuser

## Delete User
sudo userdel devuser

## Create Group
sudo groupadd devgroup

## Add User to Group
sudo usermod -aG devgroup devuser

## Switch User
su devuser

## Check Users
cat /etc/passwd

## Check Groups
cat /etc/group

## Change Ownership
chown user:user file.txt

## Change Permissions
chmod 755 file.sh
