# 07-开始手搓，开始在Fedora上编译内核

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





<figure><img src=".gitbook/assets/kernel_git_stable_linux.git.jpg" alt="" width="375"><figcaption></figcaption></figure>

切换到root用户之后，在当前目录下 创建一个Git的目录，之后在创建的Git目录里面

```
[root@fedora37 ~]# mkdir Git
[root@fedora37 ~]# cd Git/
[root@fedora37 Git]# git clone git://git.kernel.org/pub/scm/linux/kernel/git/stable/linux.git
Cloning into 'linux'...

# 在这里 国内的用户可能要久等一下

remote: Enumerating objects: 11599348, done.
remote: Counting objects: 100% (1839/1839), done.
remote: Compressing objects: 100% (797/797), done.
Receiving objects:   0% (270/11599348), 228.01 KiB | 16.00 KiB/s

# 之后这里也要等待好久



```















#### 开始手搓





#### 首次运行
