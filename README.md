#一个使用django开发的学生综合成绩管理平台.
=========================================

#项目基于django1.3.1

#实现的功能如下:

###同学的功能：
1. 登录
2. 修改密码
3. 退出
4. 在规定时间段内进行互评
5. 在规定时间段内修改互评
6. 查看自己详细信息
7. 查看自己进行的历史互评信息
8. 查看自己的互评信息(和互评排名等信息)
9. 查看成绩(包括院系、班级)
10. 对成绩的查找和排序及其他处理
11. 查看院系以班级为单位的成绩情况
12. 提交个性发展的内容
13. 查看个性发展和活动的得分情况
14. 查看综合测评成绩排名以及各种成绩组成情况详细信息
15. 对综合成绩进行查询和排序及其他处理
16. 查看院系以班级为单位的综合成绩情况)，并形成文档

###超级管理员需求：
1. 登录
2. 修改密码
3. 退出
4. 添加班级
5. 删除班级
6. 修改班级
7. 添加同学，删除同学，修改同学信息
8. 初始化同学或记录员密码
9. 开设学期互评功能,限定互评的时间段和选择学期
10. 限定每班各项名额
11. 导入成绩单
12. 查看院系以班级为单位的成绩情况
13. 对成绩的查找和排序及其他处理
14. 对个性发展的设置,添加,修改
15. 根据同学的提交和相关证明的上交，进行最终评分
16. 并根据其他信息进行加减分设置(卫生，出勤)
17. 设置成绩和日常行为分的比例情况
18. 查看综合测评成绩排名以及各种成绩组成情况详细信息
19. 对综合成绩进行查询和排序及其他处理
20. 查看院系以班级为单位的综合成绩情况
21. 查看所有人的互评信息

###搭建方法
* 下载最新版本
* 在mysql数据库中建一个comperformance数据库，然后导入sql
* 修改settings中的DATABASES
* sudo easy_install django-grappelli
* sudo easy_install xlrd
* sudo easy_install pil
* python manage.py runserver
* 用户名：admin1990 密码：admin1990
* 登录

##安装问题

#关于验证码无法显示问题，可以参考：

* http://www.douban.com/group/topic/12636401/
* http://stackoverflow.com/questions/3544155/need-help-with-a-pil-error-ioerror-decoder-zip-not-available

#启动错误问题
* No module named _imagingft
<br>
1. 先安装freetype
$ wget http://nchc.dl.sourceforge.net/project/freetype/freetype2/2.4.7/freetype-2.4.7.tar.gz
<br>
$ tar -xvzf freetype-2.4.7.tar.gz
<br>
$ cd freetype-2.4.7/
<br>
$ ./configure --prefix=/usr/local
<br>
$ make
<br>
$ make install
<br>
2. 安装PIL
<br>
下载PIL源码地址http://effbot.org/downloads/Imaging-1.1.6.tar.gz，解压进入目录python set.py install
<br>

