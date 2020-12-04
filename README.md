# 下载
`docker pull zjw201x/summerlnmp`
# 初始密码(Default password)
`cat /var/log/mysqld.log|grep 'A temporary password'`
或
password=`cat /var/log/mysqld.log|grep 'A temporary password'`;password=${password:91};echo $password
初始化(initialize)
# 请及时修改Mysql的密码(默认并未重置密码和初始化)
password=`cat /var/log/mysqld.log|grep 'A temporary password'
password=${password:91}
echo -e "${password}\n${password}\n${password}\nn\ny\ny\ny\ny\n"
# 以上三条命令的输出为以下命令的输入
mysql_secure_installation

# 警告(Warning)
> 1.请保持清醒头脑，明确自己是在容器内还是在服务器本身执行命令，以及-v挂载对文件的影响，以免造成不可挽回的损失
> 2. 当前Node和Python较火，故增加了对node.js的支持，是否添加对Python3.8的支持请在群内踊跃投票~~~
#配置(Config)
配置文件路径(Config file path)
### Nginx
/usr/local/nginx/conf/nginx.conf
### MySQL
/etc/my.cnf
### PHP
/usr/local/php7/lib/php.ini
/usr/local/php7/etc/php-fpm.conf
/usr/local/php7/etc/php-fpm.d/www.conf
