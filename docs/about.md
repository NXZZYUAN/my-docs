# 关于本项目

## 项目目标

实现从 Markdown 文档到公开网站的自动化发布，并验证「推送文档 → 自动构建 → 自动部署 → 网页更新」这条链路。

## 技术组成

| 工具 | 作用 |
| --- | --- |
| Markdown | 编写文档内容 |
| MkDocs Material | 将文档构建成静态网站 |
| GitHub Actions | 自动执行安装、构建和部署 |
| GitHub Pages | 托管并提供网站访问地址 |

## 为什么选择这套方案

MkDocs 的配置集中在 `mkdocs.yml`，页面之间的导航由 `nav` 统一维护，适合结构固定的课程文档。Material 主题自带中文界面、搜索和代码高亮，能够直接在构建产物中检查最终效果。

GitHub Actions 负责把本地验证过的构建命令原样搬到云端执行，因此本地 `mkdocs build --strict` 通过，通常云端也能通过。Pages 只负责托管构建产物，不参与内容生成，分工清晰。

## 与仓库其他部分的关系

- 网站内容在 `docs/`。
- 过程报告在 [report/README.md](../report/README.md)（GitHub 仓库内查看）。
- 本地预览命令见[使用指南](guide.md)。
