# Advanced Linux Commands

## GREP (Search)
grep "text" file.txt
grep -i "text" file.txt
grep -r "text" /directory
grep -v "text" file.txt

## FIND (Search files)
find / -name file.txt
find / -type f
find / -size +10M
find / -mtime -7

## AWK 
awk '{print $1}' file.txt
awk '{print $1, $2}' file.txt
awk -F ':' '{print $1}' /etc/passwd

## SED (Stream editor)
sed 's/old/new/g' file.txt
sed -n '1,5p' file.txt
sed -i 's/old/new/g' file.txt

## Process Management
ps aux
top
htop
kill -9 PID
pkill process_name

## Disk & System Monitoring
df -h
du -sh *
free -m
uptime

## Networking Commands
ping google.com
curl http://example.com
wget http://example.com/file
netstat -tulnp
ss -tulnp

## Permissions & Ownership
chmod 755 file.sh
chown user:user file.txt
