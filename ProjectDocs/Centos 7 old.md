## Centos 7停止支持后

### 支持CentOS7全系列更换YUM源，阿里云YUM源作为主要仓库，Vault源作为备份仓库。

```python
curl -O https://github.com/douyaolai/Blockchain-Exchange-Changelog/blob/main/ProjectDocs/yumcentos7.sh && chmod +x yumcentos7.sh && ./yumcentos7.sh
```

### CentOS 7在2024年6月30日官方停止维护，需要先执行以下命令才能执行安装宝塔命令：

```bash
sed -i 's/mirrorlist/#mirrorlist/g' /etc/yum.repos.d/CentOS-*
sed -i 's|#baseurl=http://mirror.centos.org|baseurl=http://vault.centos.org|g' /etc/yum.repos.d/CentOS-*
```

### 宝塔7.6开心版版本
`yum install -y wget && wget -O install.sh http://v7.hostcli.com/install/install_6.0.sh && sh install.sh`



> update 2024-8-5
