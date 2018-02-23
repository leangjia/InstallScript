# [Odoo](https://www.odoo.com "直达Odoo官网") 一键安装脚本

基于歪国友人： André Schenkels (https://github.com/aschenkels-ictstudio/openerp-install-scripts)
基于上述原创并做创新改进。本一键安装脚本允许您自定义 xmlrpc_port 端口、自定义原生位于/etc目录下的.conf配置文件路径。
更加强大的是此一键安装脚本允许多版本odoo共存一台服务器。强大啊！

## 安装

##### 1. 下载命令:
```
sudo wget https://raw.githubusercontent.com/Yenthe666/InstallScript/11.0/odoo_install.sh
```
##### 2. 修改相关参数：
相关参数罗列如下:<br/>
```OE_USER``` 系统用户账号名称。<br/>
```INSTALL_WKHTMLTOPDF``` set to ```False``` if you do not want to install Wkhtmltopdf, if you want to install it you should set it to ```True```.<br/>
```OE_PORT``` odoo端口,比如 8069。<br/>
```OE_VERSION``` 所要安装的odoo版本号, 例如 ```11.0``` 表示 Odoo V11， ```10.0``` 表示 Odoo V10， ```8.0``` 表示 Odoo V8。<br/>
```IS_ENTERPRISE``` 企业版 Enterprise version on top of ```11.0``` if you set it to ```True```, set it to ```False``` if you want the community version of Odoo 11.<br/>
```OE_SUPERADMIN``` 为odoo系统管理员比如admin<br/>

#### 3. 给权限脚本运行：
```
sudo chmod +x odoo_install.sh
```
##### 4. 运行脚本:
```
sudo ./odoo_install.sh
```
