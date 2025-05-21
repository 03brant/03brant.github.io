Brant的博客
本指南将介绍如何通过克隆 HuxPro 的 GitHub 仓库来快速搭建属于自己的个人博客。
🚀步骤一：Fork HuxPro 仓库
打开 HuxPro 仓库：https://github.com/Huxpro/huxpro.github.io
点击右上角的 Fork，将其复制到你自己的 GitHub 账户下。
🛠步骤二：克隆你的仓库
git clone https://github.com/你的用户名/huxpro.github.io.git
cd huxpro.github.io
🔧 步骤三：安装依赖
确保你已经安装了 Ruby 环境后，安装 Jekyll 和 Bundler：
gem install jekyll bundler
bundle install
🔄 步骤四：本地运行博客
启动本地服务器以预览博客：
bundle exec jekyll serve
打开浏览器，访问：
http://localhost:4000
你应该可以看到博客模板已经运行成功。

✍️ 步骤五：修改博客内容
修改 _config.yml
该文件包含博客的基本配置，例如网站名称、作者、描述、社交链接等：
title: 你的博客标题
author: 你的名字
email: 你的邮箱
description: 你的博客描述
url: "https://你的用户名.github.io"
修改页面内容
文章放在 _posts/ 目录，文件命名格式为 YYYY-MM-DD-title.md

修改主页欢迎信息：index.html

自定义关于页面：about.md

自定义项目展示页面：_pages/projects.md

☁️ 步骤六：部署到 GitHub Pages
确保你的仓库命名为 你的用户名.github.io，GitHub 会自动部署你的站点。

每次更新内容后：
git add .
git commit -m "更新博客内容"
git push origin main
然后访问：
https://你的用户名.github.io
即可查看你的博客上线啦！