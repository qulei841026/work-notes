#Python学习

###基础工作
####IDE-PyCharm
激活破解网站: <a>http://idea.lanyus.com</a><br>
Python开发环境<br>
pycharm2018 ip 访问
Run-Edit-Configuration 中,找到Additinal options栏 ：手动写入 --host=x.x.x.x--port=xxxx

###代码风格
https://www.python.org/dev/peps/pep-0008/

###文件管理
```
    os.path.exists('') #文件夹是否存在
    os.getcwd() #当前工作路径
```

####pyenv
**pyenv是Python-Sdk的安装和管理工具**

```
pyenv install 3.5.2
pyenv versions
pyenv local 3.5.2
```
####flask
python框架

####flask-蓝图
蓝图通俗理解就是对于视图方法模块化的一个很好的工具<br>
避免app.py过于臃肿

####requests
网络请求库

####flask-APScheduler
定时任务

####redis
数据缓存<br>
客户端src文件夹下，redis-cli<br>
from flask_cache import Cache
安装插件：pip install Flask-Cache<br>

####flask_script
flask控制台命令输入框架
```
manager = Manager(app)
if __name__ == '__main__':
    manager.run()
```

####flask_migrate
flask数据库迁移框架

####flask-mysql
```
pip install pymysql
pip install flask-sqlalchemy
```
#####创建表
```
python manager.py shell
from app import db 
db.create_all()
```






####WSGI & uwsgi
https://www.jianshu.com/p/679dee0a4193
###相关问题
####Mac系统下安装的Python3所在位置/usr/local/bin



