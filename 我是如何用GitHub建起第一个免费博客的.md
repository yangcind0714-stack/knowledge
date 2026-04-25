# 我是如何用 GitHub 建起第一个免费博客的（零代码）

> 一个完全不懂代码的人，也能在 30 分钟内拥有自己的免费博客

## 为什么要写这篇？

我是一个完全不懂代码的人。

以前总觉得“搭建博客”是程序员才能做的事 —— 要买服务器、要写代码、要配环境，听起来就很劝退。

但今天我成功了！

我的博客地址：https://yangcind0714-stack.github.io/knowledge/

这篇文章就是记录我踩过的坑和最终的方法，希望能帮到和我一样的初学者。

---

## 准备工作（不需要任何安装）

只需要一样东西：**一个 GitHub 账号**

- 去 github.com 注册（免费）
- 记住你的用户名

我就是这么开始的，没有装任何软件。

---

## 第一步：创建一个仓库

仓库（Repository）可以理解成一个**存放文件用的网盘文件夹**。

操作：
1. 登录 GitHub
2. 点击右上角的 **+** → **New repository**
3. Repository name 填：`knowledge`（也可以填其他名字）
4. 点击 **Create repository**

完成！你已经有了一个存放博客内容的“文件夹”。

---

## 第二步：开启 GitHub Pages（让它变成网站）

仓库默认只是存文件的地方，需要开启一个叫 GitHub Pages 的功能，才能让别人通过网址访问。

操作：
1. 进入仓库，点击 **Settings**
2. 左侧菜单点击 **Pages**
3. 在 Branch 那里，把 `None` 改成 `main`
4. 点击 **Save**

等 1-2 分钟，你会看到一个绿色提示框：
> Your site is live at https://你的用户名.github.io/仓库名/

到这里，你的博客网址就已经生效了！

---

## 第三步：写第一篇文章

GitHub 上写文章非常简单，不需要任何编辑器。

操作：
1. 点击 **Add file** → **Create new file**
2. 文件名写：`my first paper`
3. 内容写：
4. 4. 底部小框写一句说明（比如"写第一篇文章"）
5. 点击 **Commit changes**

文章就保存成功了。

---

## 第四步：创建首页（解决 404 问题）

一开始我直接访问博客网址，结果看到 **404**。

原因是：GitHub Pages 需要一个叫 `index.html` 或 `index.md` 的文件作为首页。

解决方法：
1. 点击 **Add file** → **Create new file**
2. 文件名写：`index.html`
3. 内容复制下面的代码：

```html
<!DOCTYPE html>
<html>
<head>
 <meta charset="UTF-8">
 <title>我的知识博客</title>
</head>
<body>
 <h1>我的知识博客</h1>
 <p>欢迎来到我的博客！</p>
 
 <hr>
 
 <h2>文章列表</h2>
 <ul>
     <li><a href="my first paper">第一篇文章</a></li>
 </ul>
</body>
</html>
