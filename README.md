# my-docs

个人文档网站：使用 MkDocs Material 编写四页文档，通过 GitHub Actions 自动构建并部署到 GitHub Pages。

- 网站地址：https://nxzzyuan.github.io/my-docs/
- 个人实验报告：[report/README.md](report/README.md)
- 本站内容：[docs/](docs/)

## 本地预览

```bash
python -m venv .venv
source .venv/Scripts/activate
python -m pip install -r requirements.txt
python -m mkdocs serve
```

浏览器打开 `http://127.0.0.1:8000/`。

## 目录

| 路径 | 作用 |
| --- | --- |
| `docs/` | 网站源文档 |
| `site/` | 本地构建产物，不提交 |
| `report/` | 实践过程报告与截图 |
| `.github/workflows/deploy.yml` | Pages 自动部署工作流 |
