# Django-Vue3-Admin

[![img](https://img.shields.io/badge/license-MIT-blue.svg)](https://gitee.com/liqianglog/django-vue-admin/blob/master/LICENSE)  [![img](https://img.shields.io/badge/python-%3E=3.7.x-green.svg)](https://python.org/)  [![PyPI - Django Version badge](https://img.shields.io/badge/django%20versions-3.2-blue)](https://docs.djangoproject.com/zh-hans/3.2/) [![img](https://img.shields.io/badge/node-%3E%3D%2012.0.0-brightgreen)](https://nodejs.org/zh-cn/) [![img](https://gitee.com/liqianglog/django-vue-admin/badge/star.svg?theme=dark)](https://gitee.com/liqianglog/django-vue-admin)

[预 览](https://demo.dvadmin.com) | [官网文档](https://www.django-vue-admin.com) | [群聊](https://qm.qq.com/cgi-bin/qm/qr?k=fOdnHhC8DJlRHGYSnyhoB8P5rgogA6Vs&jump_from=webapi) | [社区](https://bbs.django-vue-admin.com) | [插件市场](https://bbs.django-vue-admin.com/plugMarket.html) | [Github](https://github.com/liqianglog/django-vue-admin)




* 🧑‍🤝‍🧑前端采用 Vue3+TS+pinia+fastcrud(感谢[vue-next-admin](https://lyt-top.gitee.io/vue-next-admin-doc-preview/))
* 👭后端采用 Python 语言 Django 框架以及强大的 [Django REST Framework](https://pypi.org/project/djangorestframework)。
* 👫权限认证使用[Django REST Framework SimpleJWT](https://pypi.org/project/djangorestframework-simplejwt)，支持多终端认证系统。



## 前端

```bash
# 克隆项目
git clone https://gitee.com/huge-dream/django-vue3-admin.git

# 进入项目目录
cd web

# 安装依赖
npm install -g yarn
yarn install --registry=https://registry.npm.taobao.org

# 启动服务
yarn run dev
# 浏览器访问 http://localhost:8080
```



## 后端

~~~bash
1. 进入项目目录 cd backend
2. 在项目根目录中，复制 ./conf/env.example.py 文件为一份新的到 ./conf 文件夹下，并重命名为 env.py
3. 在 env.py 中配置数据库信息
	mysql数据库版本建议：8.0
	mysql数据库字符集：utf8mb4
4. 安装依赖环境
	pip3 install -r requirements.txt
5. 执行迁移命令：
	python3 manage.py makemigrations
	python3 manage.py migrate
6. 初始化数据
	python3 manage.py init
7. 初始化省市县数据:
	python3 manage.py init_area
8. 启动项目
	python3 manage.py runserver 0.0.0.0:8000
或使用 daphne :
  daphne -b 0.0.0.0 -p 8000 application.asgi:application
~~~

## 访问项目

- 访问地址：[http://localhost:8080](http://localhost:8080) (默认为此地址，如有修改请按照配置文件)
- 账号：`superadmin` 密码：`admin123456`

