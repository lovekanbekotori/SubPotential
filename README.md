# SubPotential - 便捷地在线订阅您的产品和服务  
[演示站(同时也是官方运营站)](https://platform.zixutech.cn/) | [QQ群](//shang.qq.com/wpa/qunwpa?idkey=b58840392faae59978a8250dd5bf21d71c570e025a7499b405d273ee2f75402b)  
本产品基于ThinkPHP5 开发，能够让您方便的出售和管理您的产品及服务
  
目前已实现独特特性：  
1、快速将您的产品或服务作为产品发布至首页，仅需简单几步信息填写。  
2、为方便对接QQ机器人，支持产品绑定QQ群号码。  
3、为每个产品设置不同的价格和期限方案。  
4、支持添加优惠券，对您的产品进行“打折”。  
5、在线扫码充值。  
6、全平台响应式布局。  
7、前台使用精美的Material UI风格。  
8、用户组基础权限管理。  
9、完善的工单系统（支持添加指定用户为客服，可处理工单，支持工单评价）。  
  
ToDo List  
For Pro:  
□ 邀请链接返利功能。  
For Public:  
○ 修复和完善。
  
###### 小提示：目前本产品刚开发完毕，不排除有很多BUG的可能性，如果您在使用中遇到问题，您可以通过一下途径直接向作者联系！  
Email: zixutech@gmail.com  
QQ号码：644752622  
###### 或者您也可以通过官方演示站发表工单提交问题，也是作者本人亲自处理哦！  
  
# 环境需求  
PHP 5.6+ with MYSql 5.6+  
Curl扩展  
支持集成式环境(LAMP，LNMP，MAMP等)
# 安装说明  
##### 安装程序
将本项目全部下载后，直接上传至您网站**根目录**，请不要上传至二级目录哦。  
将mysql.sql导入到您的数据库，至此安装完成。  
##### 文件权限  
runtime 目录需要设置为777权限
##### URL重写  
对于Apache服务器，您不需要进行什么特殊的配置，因为本产品使用MAMP作为开发环境。  
但对于Nginx的服务器，您需要将您的重写按以下内容配置  
```  
location / {
   if (!-e $request_filename) {
   rewrite  ^(.*)$  /index.php?s=/$1  last;
   break;
    }
 }
```  
同时您需要将您的Nginx配置文件的root字段后面加上public，如下所示(官方站的配置)  
```  
root /www/wwwroot/platform.zixutech.cn/public;
```  
推荐您使用[宝塔面板](https://www.bt.cn/)对您的网站进行管理。  
使用宝塔面板仅需在网站 -> 设置 -> 伪静态 内修改为Thinkphp方案，并在配置文件中修改一下第7行root如上述所说配置即可。  
##### 安装完成  
前台地址：您的域名/index   后台地址：您的域名/admin  初始用户名/密码：admin/admin  
修改密码或添加管理员，请到数据库内手动修改admin表。  
##### 后续操作  
以下操作不是必须的，但仍推荐你完成这些操作：  
  
修改初始管理员账号密码  
到 网站设置-基本配置 中将站点URL修改为您自己的，如果不更改，系统将无法正常接受回调请求。  
给本项目一个Star~  
  
# 其他
#### 本Github项目为SubPotential Public (大众免费版)，功能与 SubPotential Pro 未来在功能和完善程度上有所区别（请继续查阅下一栏目）。 
#### 本项目仅供演示和测试使用，如果您有更多需求，请联系我购买SubPotential Pro许可证，来获取更加完善服务和更新。
#### *未来针对于 Pro 版本的更新将不会应用于 Public 版本，而针对 Public 的更新将全部应用于 Pro 。*
  
# 产品许可证  
#### 目前 SubPotential Pro 仍处于完善阶段，我们希望为您提供一个非常完善而不是漏洞百出的产品。您目前可以通过前期预售来购买 Pro 许可证。  
#### 具体许可证价格请到[官方网站](https://blog.zixutech.cn)进行查阅。
  
# 版本区别  
2018年10月21日 - 产品刚发布，免费版和专业版无功能差别。
