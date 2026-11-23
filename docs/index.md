# 我的技术文档

欢迎访问我的个人文档网站。本网站使用 MkDocs 构建，通过 GitHub Actions 自动部署到 GitHub Pages。

- 作者：NXZZYUAN
- 实践主题：静态文档自动部署
- [关于本项目](about.md)
- [使用指南](guide.md)
- [API 参考](api.md)

## 这个网站在做什么

这个站点是「系统分析与设计」课程第二次平时作业的交付物。它把四份 Markdown 文档编译成静态网站，并由 GitHub Actions 在每次推送后自动完成构建与发布。

| 环节 | 使用的工具 | 产物 |
| --- | --- | --- |
| 编写内容 | Markdown | `docs/` 下的四个页面 |
| 本地构建 | MkDocs + Material 主题 | `site/` 静态文件 |
| 自动构建与部署 | GitHub Actions | Actions 运行记录 |
| 在线访问 | GitHub Pages | 公开网站地址 |

## 实践体会

第一次把「写文档」和「发布网站」分开理解：日常只维护 `docs/` 下的源文件，`site/` 由工具生成，不需要手工修改。这样文档可以像代码一样提交、审查和回滚。
