# Gaming-Direct Sing-box Rules (Release Based)

这是一个基于 **GitHub Release** 的游戏规则集仓库。支持从 JSON 自动编译为二进制（SRS）并作为发布附件（Assets）托管。

## 如何在 Sing-box 中引用

由于我们使用 Release 进行托管，引用链接将始终指向最新版本的二进制文件：

```json
{
  "tag": "Gaming-Direct",
  "type": "remote",
  "format": "binary",
  "url": "https://github.com/TextlineX/GameRules/releases/latest/download/Gaming-Direct.srs",
  "download_detour": "🚀 自动选择"
}
```

## 如何触发发布一个新的 Release

当你修改了 `src/` 下的内容后，通过以下 Git 指令发布新版本：

1.  `git add .`
2.  `git commit -m "feat: update game rules"`
3.  `git tag v1.0.1` (版本号根据你的情况递增)
4.  `git push origin main --tags`

推送 **Tag** 后，GitHub 会自动创建一个包含编译好的 `.srs` 文件的 Release。
