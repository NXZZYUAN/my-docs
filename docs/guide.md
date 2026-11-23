# 使用指南

1. 修改 `docs` 目录中的 Markdown 文件。
2. 在本地预览并检查页面及链接。
3. 提交修改并推送到 `main` 分支。
4. 在 Actions 页面查看构建与部署状态。
5. 打开网站检查内容是否更新。

## 常用命令

```bash
python -m venv .venv
source .venv/Scripts/activate
python -m pip install -r requirements.txt
python -m mkdocs serve
python -m mkdocs build --strict
```

`mkdocs serve` 用于本地预览，默认地址是 `http://127.0.0.1:8000/`；`mkdocs build --strict` 会在出现警告时返回失败，适合在推送前自检。

## 页面之间怎么走

- 返回[首页](index.md)
- 了解[技术组成](about.md)
- 查看[API 参考](api.md)

## 注意事项

- `nav` 中的路径相对于 `docs/`，不要写成 `docs/index.md`。
- `site/` 是构建产物，已加入 `.gitignore`，不手工修改。
- 只修改 `report/` 或 `README.md` 不会触发部署，这是工作流按路径过滤的预期行为。
