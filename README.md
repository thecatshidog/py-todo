# py-todo
this is a py-flask-restful test demo repository.

v0.2
1、flask-script是自定义shell的作用，起到管理整个应用的作用，自动化运维

2、通过在一个txt文件中写入项目依赖，可以通过pip安装

```
pip install -r package.txt
```

感觉就像是nodejs的package.json。

3、jinja这个模板也就是和ejs差不多，通过{{}}这个插值符号来进行判断，而且还能写入一些逻辑程序

4、不要在项目中命名flask.py,这样会有冲突

5、
通过下面这个方式可以让外网访问，本地还是视同localhost来访问
```
app.run(host='0.0.0.0')
```
0.0.0.0不是一个单纯的IP地址，他指的是所有不清楚的主机和目的网络。这里的不清楚指的是路由表中没有指定如何到达。反正不知道的东西都在这里。
0.0.0.0其实也代表了本机的所有可用接口。
通过ipconfig来知道本机的IP地址。

6、render_tempate是实现模板渲染的方法，它会在同级的template下寻找模板

```
--__init__.py
--template/
```
7、git tag小贴士：

```
// 生成tag标签，其实就是一个打包的版本
git tag -a v0.1 -m "change log"

// 删除错误的tags版本
git tag -d <tagname>
git push origin :refs/tags/<tagname>

// 查看所有的tags
git tag
```
