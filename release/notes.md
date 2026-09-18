# v3.10.1

## 新增功能

- Codex 主请求支持单独配置上游地址，可使用中转服务；额度、模型目录、个人资料和重置卡等辅助请求默认继续访问官方地址。
- GitHub Release 支持推送 `vX.Y.Z` 标签自动触发，按当前仓库生成 GHCR 镜像版本、`sha-*` 标签和稳定版 `latest` 标签。

## 升级说明

- 新增 `openai.api.auxiliary_base_url` 配置项；省略时使用官方 `https://chatgpt.com/backend-api`，已有配置无需修改。
- 本版本部署默认仓库为 `hiven425/codex-proxy-rs`，升级前请确认 GitHub Container Registry 权限和镜像拉取地址。
