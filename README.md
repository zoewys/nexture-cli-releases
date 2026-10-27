# Nexture 插件公开下载

DeepSeek Harness（DSH）的 Nexture CLI 与 Nexture Team 官方安装包分发仓库。

## 当前版本

- Nexture CLI：**0.2.0-alpha.45**
- Nexture Team：**0.1.0-alpha.18**

[下载最新版及安装说明](https://github.com/zoewys/nexture-cli-releases/releases/tag/v0.2.0-alpha.45) · [全部历史版本](https://github.com/zoewys/nexture-cli-releases/releases)

在 Release 的 Assets 下载两个 `.tgz`、`SHA256SUMS` 和 `INSTALL.md`，放到同一文件夹，执行 `shasum -a 256 -c SHA256SUMS`。两项显示 OK 后，在 DSH「插件 → 添加插件」选择需要的本地包并启用，待当前任务结束后正常重启。Team 可以独立安装。Source code ZIP 不是插件安装包。

公开附件无需 GitHub 账号或私有源码仓库权限。已验证 macOS Apple Silicon、DSH 0.2.1-rc.3、Node.js ≥20；CLI 使用 Herdr 0.9.5，可在插件配置内检查或安装。CLI 登录与首次钩子/目录信任由用户自行确认。

## 发布约定

安装包与 Release 统一在本公开仓库发布；私有开发仓库仅维护源码及版本标签，不再创建 Release。CLI 与 Team 版本可以独立演进，每次 Release 正文和附件清单标明各自版本。

安装包不包含账号凭据、角色记忆或任务历史。当前未发布 npm，未自动上架 DSH 插件目录。UNLICENSED。
