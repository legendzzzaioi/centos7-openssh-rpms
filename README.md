# centos7-openssh-rpms
centos7 openssh rpms

### References
[boypt/openssh-rpms](https://github.com/boypt/openssh-rpms)

### Upgrade
To upgrade OpenSSH on CentOS 7 using the provided RPMs or compiling your own, then
```
yum localinstall ./openssh-*.rpm
chmod 600 /etc/ssh/ssh_host_rsa_key /etc/ssh/ssh_host_ecdsa_key /etc/ssh/ssh_host_ed25519_key
systemctl start sshd
```
