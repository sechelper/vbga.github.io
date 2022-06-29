#  VBGA (Vulnerabilities beginner guide app)

漏洞入门指南应用程序（VBGA）是一个集成所有Web应用基础漏洞的程序。其主要目标是帮助安全人员在法律允许的条件下入门学习渗透技能，并帮助教师/学生在真实的漏洞环境内教授/学习基础web应用程序安全知识。

## 安装使用

由于目前VBGA还不是很成熟，暂时闭源管理，但我们可以为您提供安装包，预计22年底前会开源，扫描二维码加入群聊。

![vulab-vbga](https://official-accounts.oss-cn-beijing.aliyuncs.com/img/qrcode/vulab-vbga.png)

### 使用vulab靶场安装

[vulab靶场]()快速启动`VBGA`环境，创建`vbga.yml`文件写入以下内容

```yml
version: "3.3"
services:
  vbga:
    image: sechelper/vulab:vbga-v1.0.0
    ports:
      - 8080:8080
      - 3306:3306
    volumes:
      - /opt/jdk-17.0.3.1/:/opt/jdk17
```

启动实验环境

```bash
sudo docker-compose -f vbga.yml up
```

### 免责声明

我们不对任何人使用VBGA行为负责，在前文已经明确此应用程序的目的。禁止将VBGA安装到生产环境内，如果您的服务器由于安装 VBGA受到损害，我们对此没有任何的责任，而是安装管理人的责任。
