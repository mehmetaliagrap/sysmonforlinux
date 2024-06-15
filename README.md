# sysmonforlinux
sysmon for linux


# # sysmon offline installation on Linux Red Hat 8.8 
	root@xxx:/]# /cat /etc/redhat-release
 		Red Hat Enterprise Linux release 8.8 (Ootpa)
	root@xxx:/tmp]# cd /tmp/
	root@xxx:/tmp]# rpm -Uvh sysinternalsebpf-1.3.0-0.el8.x86_64.rpm
	root@xxx:/tmp]# rpm -Uvh sysmonforlinux-1.3.3-0.el8.x86_64.rpm
	root@xxx:/tmp]# sysmon -accepteula -i SysmonForLinux-CollectAll-Config.xml
	root@xxx:/tmp]# systemctl status sysmon
	root@xxx:/tmp]# tail -f /var/log/messages | grep sysmon
