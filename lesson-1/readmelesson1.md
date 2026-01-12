github
Git=分布式版本控制系统 （记录每次修改；随时回到之前的版本；默认只在本地工作）类似 word 的保存记录+历史版本
Github=是基于 Git 的代码托管与协作平台（存放代码；备份；给别人看作品集；协作（多人同时写代码）Issue（提问题 / 记录 bug）Pull Request（代码审查））类似给程序员用的网盘

添加新的仓库: 点击 create a new repository-choose visibility-Add README（项目说明文件，页面最先展示，对找工作非常重要）-Add .gitignore（哪些文件不要被管理，如密码文件，垃圾文件；本地配置文件；node_modules/；.DS_Store）-Add license(具有法律效益)(GPL-3.0 license GNU GENERAL PUBLIC LICENSE Version 3 （表示允许商业使用，但禁止闭源再发布，基于 GPL 的修改版本 必须继续 GPL 开源)；MIT （可商用，不用开源）

在终端下载 Homebrew,类似 APP 商店，是 Mac 的命令行软件管理器，之后下载可以用 brew install XXX: 1.打开终端：command+空格键-输入 terminal 2.复制 Homebrew 的下载地址到终端 3.同理，复制 Oh My Zsh 的下载链接到终端

问题：什么是终端 Shell？ 什么是 Zsh？
Terminal 是一个输入文字命令的窗口，它本身不干活。Shell 才是真正干活的翻译官，解释命令。常见 Shell 有 bash(老)，zsh(新)，fish。现在 macOS 默认使用 Zsh.Oh My Zsh 功能是命令补全，高亮。类比：Zsh 是安卓系统， Oh my Zsh 是华为 UI

把 GitHub 上的内容下载到本地：
1.brew install nvm - brew install node
问题 Node 是什么？JavaScript 运行环境/让 JS 能在电脑上跑（不只是浏览器）
问题 NVM 是什么？ Node Version Manager （Node 版本管理工具）
2.node -v (注意中间有空格号，得到回复 v22.14.0) （v=version+Node 版本号 说明 Node 已安装成功，当前环境可以运行 JS/前端工具）
3.git -v（回复 git version 2.39.5 表示 Git 已安装及其版本）
4.mkdir code （ 创建名为 code 的文件夹 make directory ，注意是创建文件夹，不能创建文件，code 是文件夹的名字，比如 mkdir project1）
5.ls(=list 列表，查看当前目录内容=Finder 里看到的内容) 6. open ./(打开当前目录的可视化窗口)
7.cd code （change directory 进入某个文件夹；注意这里 code 文件夹必须存在，注意大小写） cd 的变体：回到上一级目录 cd ../ 直接回到“家目录” cd ~ /连续进入多层目录 cd code/learn-web/lesson1 /看地址栏 pwd（当忘记自己在哪里时）
8.code git clone "复制 GitHub 文档右上方 code 里 HTTPS 的地址"（把 GitHub 上的远程仓库复制到本地）
问题：什么是 SSH？如何在 MAC 中配置 SSH？
SSH 是一种安全的“免密码身份验证方式”，用一对钥匙：公钥（给 GitHub），私钥（留在你电脑） 9.在 VSCODE 中添加新的文件夹 lesson-1，添加文件 index.html
10.cd ~/code/learn-web
11.git status
12.git add .
13.git commit -m"first"
14.git push
