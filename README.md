# 写一个有身份验证的web项目玩玩
# 默认使用sqlite3 数据库

# 环境搭建
使用sqlite3数据库，需要在编译之前安装sqlite，然后编译
yum install sqlite-devel -y

# 添加第三方认证登录
pip install social-auth-app-django==2.1.0
settings.py INSTALLED_APPS 中添加
'social_django',
