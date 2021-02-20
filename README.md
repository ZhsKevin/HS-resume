**Resume**---

## 一份优雅简约的在线简历

- 优化构建，页面秒开无闪烁
- 自适应屏幕兼容移动端
- 支持部署到ghpages，可在线浏览
- 自动生成 PDF，全自动化流程
- 欢迎Star

## 使用
1. 项目依赖于 Node 环境，你需要先到 Node 官网[2] 下载并安装对应系统的 Node 程序。安装好后，在命令行输入 node -v，如果出现相应的版本号，说明 Node 环境安装成功。

2. fork本项目后再使用Git工具Clone到本地修改。

3. 使用 CD 命令进入到项目目录，输入`npm install`命令，安装程序所使用的依赖环境。

4. 再输入 `npm run dev` 命令，项目会进行编译，并自动打开浏览器，加载出简历的页面。

5. 打开编辑器对简历内容进行修改。

5. 项目的整体目录结构如下：
            
            `├── README.md
                ├── node_modules
                ├── package-lock.json
                ├── package.json
                ├── postcss.config.js
                ├── src
                ├── webpack-dist.config.js
                ├── webpack.config.js
                └── webpack.js`
        
7. 修改简历内容，直接编辑 `index.html` 文件。

8. 如果要修改简历的样式，比如主题色、字体等等，需要编辑 `main.css` 文件。

9. 简历修改完后，刷新一下浏览器就可以看到最新的内容。

10. 项目部署前，需要先在 GitHub 仓库中建立一个名为 `username.github.io` 的仓库，其中 `username` 是你的 GitHub 账户名称。这个仓库可以生成一个域名，你可以在这个域名下创建仓库，将一些静态内容资源托管到上面，比如自己的博客。

11. 回到项目，在命令行中先输入`cnpm install cross-env`再输入 `npm run pub` 命令，会自动创建一个 gh-pages 分支并推送到 GitHub 的仓库。

12. 打开上面 Fork 的仓库地址，点击设置，滑动到 `GitHub Pages` 设置选项，将分支选择为 `gh-pages`。

13. 然后打开生成的网页即可看到在线的简历，将链接发给其他人，其他人通过浏览器打开可以直接访问

14. 使用快捷键 `ctrl+p` 或者 `command+p` 调用浏览器的打印功能，可以将简历导出为 pdf 格式的文件。

<<<<<<< HEAD
       

## **演示页面**

## **电脑端：**

![在这里插入图片描述](https://img-blog.csdnimg.cn/20210220155720297.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3poczI2MDEzMzE3Mg==,size_16,color_FFFFFF,t_70)

## **手机端：**

![在这里插入图片描述](https://img-blog.csdnimg.cn/20210220160017450.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3poczI2MDEzMzE3Mg==,size_16,color_FFFFFF,t_70)



### **详细说明**

### **fork & clone**

首先进入托管在 GitHub 上的简历项目主页**[1]**，点击右上角的 Fork 按钮，等待若干秒后，你的项目列表里会多出来一个同名的仓库。



![ea92bc0663eb92fbeab04c50e7e78540.png](https://img-blog.csdnimg.cn/img_convert/ea92bc0663eb92fbeab04c50e7e78540.png)

把新生成的项目用git clone 到本地，就可以开始在本地进行调试和开发了。
（gir不会的可以去查一下git使用方法）



![在这里插入图片描述](https://img-blog.csdnimg.cn/20210220160123817.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3poczI2MDEzMzE3Mg==,size_16,color_FFFFFF,t_70)


### **安装依赖**

项目依赖于 Node 环境，你需要先到 **[Node 官网](https://nodejs.org/)** 下载并安装对应系统的 Node 程序。（具体方法百度即可）

安装好后，在命令行输入 `node -v`，如果出现相应的版本号，说明 Node 环境安装成功。

![在这里插入图片描述](https://img-blog.csdnimg.cn/2021022016021349.png)

使用 `cd` 命令进入到项目目录，输入 `npm install` 命令，安装程序所使用的依赖环境。

再输入 `npm run dev` 命令，项目会进行编译，并自动打开浏览器，加载出简历的页面。

这时，就可以打开编辑器对简历内容进行修改了。

### **简历编辑**

项目的整体目录结构如下：

```
.
├── README.md
├── node_modules
├── package-lock.json
├── package.json
├── postcss.config.js
├── src
├── webpack-dist.config.js
├── webpack.config.js
└── webpack.js
```

我们只需要对 `src/` 文件夹中的文件进行修改，其他文件是项目运行的一些配置文件。

![在这里插入图片描述](https://img-blog.csdnimg.cn/20210220160346388.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3poczI2MDEzMzE3Mg==,size_16,color_FFFFFF,t_70)

如果要修改简历内容，需要编辑 `index.html` 文件。如果你有前端的基础，这应该很好上手。

找到模版中对应的位置，比如个人信息部分，把中文内容改成自己的就行了。
举个例子 这里面的名字改成你的名字就行
```javascript
<header class="content-hd">
      <section class="title">
        <div class="name">
          <h1>张得帅</h1>
        </div>
      </section>
      <section class="info">
        <ul>
          <li>求职意向：Java开发工程师</li>
          <li>所在城市：XX省XX市</li>
          <li>出生年月：1XXX 年 XX 月</li>
          <li>联系方式：XXX-XXX-XXX</li>
          <li>
            个人邮箱：<a href="mailto:Zhss1004@163.com">XXXXX@163.com</a>
          </li>
<!--          <li>-->
<!--            GitHub：<a href="https://github.com">github.com</a>-->
<!--          </li>-->
        </ul>
      </section>
    </header>
```

如果要修改简历的样式，比如主题色、字体等等，需要编辑 `main.css` 文件。

比如我将简历主题色改为别的颜色，只需要下载取色器然后更改一行代码。

```javascript
$theme-color: #126ab8;
```

简历修改完后，刷新一下浏览器就可以看到最新的内容。

### **项目部署**

**替换webpack-dist.config.js文件里的yourwebsite.com为你自己的域名，并根据该文档配置你的域名解析 （这一步如果你没有自己的网页，则把这一行注释，这样系统生成的GitHubpages则默认设置为网址https://yourname.github.io/MyResume/ 这个域名也可以用但是太low了，建议个人主页去买一个域名，阿里云新人域名一年一块钱很方便）**

![在这里插入图片描述](https://img-blog.csdnimg.cn/20210220161653630.png)

回到项目输入 npm run pub 命令，会自动创建一个 gh-pages 分支并推送到你fork的 GitHub 的仓库。
（如果有什么启动不了的错误是环境问题，可以尝试回到项目，在命令行中先输入cnpm install cross-env再输入 npm run pub 命令）

打开上面 Fork 的仓库地址，点击设置，往下滑动到 `GitHub Pages` 设置选项，将分支选择为 `gh-pages`。此时上面的网站就是我说的设置域名，如果你没有设置域名则这个地方应该是https://yourname.github.io/MyResume/ 
![在这里插入图片描述](https://img-blog.csdnimg.cn/20210220162159376.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3poczI2MDEzMzE3Mg==,size_16,color_FFFFFF,t_70)


然后打开刚才显示的网页即可看到在线的简历，将链接发给其他人，其他人通过浏览器打开可以直接访问

使用快捷键 `ctrl+p` 或者 `command+p` 调用浏览器的打印功能，可以将简历导出为 pdf 格式的文件。


希望大家在都能找到满意的工作。
=======
>>>>>>> 84960c5afaf9d60674e8dca018274e21dc109995
