用法（一步步）
解压：

bash
复制
编辑
unzip my_blog_starter.zip
cd my_blog
拉取 PaperMod 主题（需要 git）：

bash
复制
编辑
bash setup_theme.sh
本地预览（需要安装 Quarto 与 Hugo）：

bash
复制
编辑
# 渲染 Quarto 内容到 content/
cd analysis && quarto render && cd ..

# 启动 Hugo 预览
hugo server -D
浏览器打开提示地址（默认 http://localhost:1313）。

初始化并推送到你的 GitHub 仓库 QianhuiWan/my_blog：

bash
复制
编辑
git init
git add .
git commit -m "Init Quarto + Hugo PaperMod site"
git branch -M main
git remote add origin https://github.com/QianhuiWan/my_blog.git
git push -u origin main
开启 GitHub Pages：

打开仓库 → Settings → Pages

选择部署分支：gh-pages（CI 会自动创建）

等工作流跑完，你的网站就上线啦

需要我把站点标题、菜单或 PaperMod 的外观（比如默认深色/浅色、头像、社交链接）再帮你改改吗？告诉我你想要的标题/头像 URL/社交链接，我给你直接调好配置。



