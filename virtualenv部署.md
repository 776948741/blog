# virtualenv部署  
## yum安装相关依赖和python-pip程序  
```bash  
[root@9aa3b82f4987 ~]# yum install epel-release -y
[root@9aa3b82f4987 ~]# yum install python-pip  
```

## 安装virtualenv环境  
```bash
[root@9aa3b82f4987 ~]# pip install virtualenv
```  

## 建立并切换到项目目录  
```bash  
[root@9aa3b82f4987 ~]# mkdir -p /data/testpj && cd /data/testpj/
[root@9aa3b82f4987 testpj]# virtualenv venv
New python executable in /data/testpj/venv/bin/python2
Also creating executable in /data/testpj/venv/bin/python
Installing setuptools, pip, wheel...done.
[root@9aa3b82f4987 testpj]# cd venv/
[root@9aa3b82f4987 venv]# source bin/activate
(venv) [root@9aa3b82f4987 venv]#  
```

## 可以在测试环境安装相关的python库了，这里面的和外边的系统不冲突

