#关于流程

首先进入vscode，在文稿中打开mdbook-site

1.本地编译命令
rm -rf book

mdbook serve

后control+c关闭本地网址。

2.以下为提交至git的命令

mdbook build

git add .

git commit -m "更新文档内容"

git push origin main