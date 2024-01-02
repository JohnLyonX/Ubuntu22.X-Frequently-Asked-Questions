# Ubuntu22.X-Frequently Asked Questions

1. Q: How to configure an independent IP for my Ubuntu system?
   - A: Edit using Vim, /etc/netplan/xx-installer-config.yaml, Configuration content reference file: xx-installer-config.yaml

2. Q: How do I get my Ubuntu system to allow connecting as root when connecting using ssh?
   - A: The file that needs to be modified is: /etc/ssh/sshd_config, find “#PermitRootLogin prohibit-password” changed to “PermitRootLogin yes”, if content is null or not folder, You need install ssh (apt install ssh)
