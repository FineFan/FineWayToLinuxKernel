# 06-找个车库 开始手搓发动机

## 首先你需要一个车库。

这里说的车库其实就是一台自己的Fedora Workstation。我知道大部分人在实际工作中 其实用的都是 Microsoft 公司出品的 Windows系统。









## 之后，整理一下你的车库

这里说明一下 在安装成功之后你需要对你的系统进行哪些调整，来完成你的桌面工作站的配置。









## 开始手搓

接下来我们就开始尝试亲手编译一个内核 并启动。

#### 准备零件

首先，我们需要拿到上游供应商的零件。



{% embed url="https://kernel.org/" %}



<figure><img src=".gitbook/assets/Kernel.org_main_page.jpg" alt=""><figcaption></figcaption></figure>









#### 准备工具





以下是你需要的工具。

vim&#x20;

gcc

make

git

wget





```shell
// Some code
dnf -y install gcc vim make git wget


[fine@fedora37 ~]$ sudo su - root
[sudo] password for fine: 
[root@fedora37 ~]# dnf -y install wget gcc make vim

```





<figure><img src=".gitbook/assets/kernel_git_stable_linux.git.jpg" alt=""><figcaption></figcaption></figure>

#### 开始手搓





#### 首次运行
