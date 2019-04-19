:running:Blog:running:
============

好好学习，天天向上。

## 目录

* [项目背景](#项目背景)
* [安装git](#安装git)
* [安装node](#安装node)
* [安装淘宝镜像cnpm](#安装淘宝镜像cnpm)
* [本地运行](#本地运行)
* [打包上传运行](#打包上传运行)

## 项目背景

刚接触 GitHub 的时候就开始在仓库里创建 [Issues] 来记录学习笔记，那时候我还不知道有 GitHub Pages，后来了解到了可以通过 GitHub Pages 来搭建 [个人博客站点]，但是如果涉及到在文章里嵌套图片的话还是比较麻烦的

通过 Issues 记录学习笔记的优点：

- [x] 在线编辑和预览，随时添加和提交（不用担心电脑坏了导致笔记丢失）
- [x] 当笔记里到嵌套图片时，支持粘贴屏幕截图和拖拽添加图片
- [x] 带有搜索和排序功能
- [x] 可通过 Label 来对 Issues 进行分类
- [x] 可以把每一个 Comment 作为一个小的知识点不停的追加到 Issue 里
- [x] 结合 GitHub Pages 绑定域名来搭建个人博客站点

## Demo

> [个人博客](https://jaysleo.github.io/mblog)

## 使用方法

#### 下载项目到本地
```
git clone https://github.com/jaysleo/Blog.git
```
#### 本地运行

> 1.安装依赖

```
npm install
```
安装了cnpm就用
```
cnpm install
```

> 2.在本地开启服务，然后就可以通过 http://localhost:8084 访问了

```
npm run dev
```

> 3.个人配置 - 修改「vue/src/store/account.js」文件中的「state」属性


> 4.个人配置 - 修改网站图标

```
修改「vueeBlog/static/img/favicon.ico」文件
```
> 5.个人配置 - 修改网站标题

```
修改「vue/index.html」文件里「<title>」标签里的内容
```

#### 发布到 GitHub Pages

> 1.打包

```
npm run build
```
> 2.发布

```
拷贝「Blog/docs」目录里的所有文件到「GitHub Pages」的根目录下
并将「GitHub Pages」仓库 PUSH 到 GitHub 上
```
#### 打包发布小白详细步骤

> 1.在GitHub 上创建一个仓库 [myblog]

> 2.把myblog 检出到本地

> 3.把打包好的「Blog/docs」目录里的所有文件拷贝到「myblog」的根目录下

> 4.git bash 按顺序执行以下命令
```
安装git后配置
git config --global user.name "你的github用户名"

git config --global user.email "你的github绑定的邮箱"
```

4.1.`git status`

4.2.`git add .`

4.3.`git status`

4.4.`git commit -m "modify"`

4.5.`git pull`

4.6.`git push`
