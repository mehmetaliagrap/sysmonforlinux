# sysmonforlinux
sysmon for linux

# # sysmon offline installation on Linux Red Hat 8.8 
cat /etc/redhat-release
cd /tmp/
ls
rpm -Uvh sysinternalsebpf-1.3.0-0.el8.x86_64.rpm
rpm -Uvh sysmonforlinux-1.3.3-0.el8.x86_64.rpm
sysmon -h
ls
sysmon -accepteula -i SysmonForLinux-CollectAll-Config.xml
systemctl status sysmon
tail –f /var/log/Syslog | grep sysmon
tailf /var/log/Syslog | grep sysmon
tail -f /var/log/Syslog | grep sysmon
tail -f /var/log/| grep sysmon
tail -f /var/log/messages | grep sysmon
