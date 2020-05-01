# mysql
介绍如何安装mysql


mysql的安装分为两种，第一种是下载msi文件，相当于安装了独立的mysql环境，跟本地的计算机无直接关联
第二种，我比较推荐，下载的是zip文件，直接安装在本地，方便开发项目的时候使用。
我在用django项目的时候遇到了安装mysql的问题。



遇到的问题之一：

修改MySQL数据库的时区

输入：show variables like '%time_zone%';

输入： set global time_zone='+8:00';


遇到的经验累积：
如果django的数据库被换掉，则用户名密码也会一起失效，新的数据库建立后，需要重新配置超级用户
python manage.py cratesuperuser
