# ContentPilot 更新源

ContentPilot 专业版/Agent1.0 的更新仓库。

## 文件说明
- ersion.json — 更新清单（版本号 + 可更新文件列表），客户端启动时/--update 读取
- content_config.json — 内容配置（敏感词库 / 各平台默认文案 / 发布频率参数），热更新只需覆盖此文件
- Releases — 安装包（重装/升级用，覆盖安装保留 data 数据）

## 更新流程（档3 数据热更新）
1. 修改 content_config.json 后，把 version.json 的 version 号 +1（如 1.0.0 → 1.0.1）
2. 上传两个文件到 main 分支
3. 客户端下次启动或执行 --update 自动拉取生效，无需重装

## 版本记录
- 1.0.0 初始版本：外置敏感词/文案/频率参数