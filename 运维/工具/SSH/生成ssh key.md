#ssh

### 1.1

```shell
ssh-keygen -t rsa -b 4096 -C "your_email@example.com"
```

> 这个命令会生成一个RSA类型的4096位密钥对，并要求你提供一个关联的电子邮件地址。

### 1.2
终端会提示你输入要保存密钥对的文件路径以及一个可选的密码短语（用于保护私钥）。你可以直接按回车键接受默认的文件路径和空密码短语，也可以自定义设置。

### 1.3
密钥对生成后，终端会显示公钥的指纹（fingerprint）（The key's randomart image）和路径。默认情况下，公钥保存在<span style="color:orange"> ~/.ssh/id_rsa.pub</span>文件中。

