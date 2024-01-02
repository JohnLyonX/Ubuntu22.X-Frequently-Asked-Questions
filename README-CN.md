# Ubuntu22.X-常见问题解答

1. 问：如何为我的Ubuntu系统配置独立的IP？
    - 答：使用Vim编辑 `/etc/netplan/xx-installer-config.yaml` 文件，配置内容参考文件：`xx-installer-config.yaml`

2. 问：在使用SSH连接时，如何使我的Ubuntu系统允许以root用户身份连接？
   - 答：需要修改的文件是：`/etc/ssh/sshd_config`，找到“#PermitRootLogin prohibit-password”并更改为“PermitRootLogin yes”；如果内容为空或不存在该文件夹，您需要安装SSH（apt install ssh）。但您还应考虑是否关闭了防火墙。最后，重新加载SSH服务。
