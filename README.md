## 一份优雅简约的在线简历
- 优化构建，页面秒开无闪烁
- 自适应屏幕兼容移动端
- 支持部署到ghpages，可在线浏览
- 自动生成 PDF，全自动化流程

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

