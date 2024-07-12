# centos7-openssh-rpms
centos7 openssh rpms

### References
[boypt/openssh-rpms](https://github.com/boypt/openssh-rpms)

### Upgrade
To upgrade OpenSSH on CentOS 7 using the provided RPMs or compiling your own, then
```
[[ -f /etc/ssh/sshd_config ]] && cp -rf /etc/ssh/sshd_config /etc/ssh/sshd_config.$(date +%Y%m%d)
yum localinstall ./openssh-*.rpm -y
chmod -v 600 /etc/ssh/ssh_host_*_key
systemctl start sshd
```
