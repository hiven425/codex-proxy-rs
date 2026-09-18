# v3.10.2

## 新增功能

- GitHub Release 流程仅构建并推送多架构 Docker 镜像，不再生成二进制、安装包或 GitHub Release 附件。
- 推送匹配 `vX.Y.Z` 的标签会自动生成版本标签、`sha-*` 标签和 `latest` 标签。

## 升级说明

- Docker 镜像地址为 `ghcr.io/hiven425/codex-proxy-rs`。
- Codex 主请求与官方辅助接口的分离配置保持不变，`openai.api.auxiliary_base_url` 省略时继续使用官方地址。
