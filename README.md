# 写一个有身份验证的web项目玩玩
# 默认使用sqlite3 数据库

# 环境搭建
使用sqlite3数据库，需要在编译之前安装sqlite，然后编译
yum install sqlite-devel -y

# 安装图像处理库
pip install Pillow==5.1.0

# 添加第三方认证登录
pip install social-auth-app-django==2.1.0
settings.py INSTALLED_APPS 中添加
'social_django',

# 创建缩略图，需要的扩展
pip install sorl-thumbnail==12.4.1
settins.py 添加设置
   'sorl.thumbnail',

# 修改网站域名需要修改一下文件中的域名
images/static/js/bookmarklet.js 
images/templates/bookmarklet_launcher.js
bookmarks/setting.py
