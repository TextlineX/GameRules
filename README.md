# GameRules - 游戏规则

游戏相关分流规则，支持多客户端。

## 规则列表

| 文件 | 说明 | 行为 |
|------|------|------|
| `kg-mc.json` | 库洛/鸣潮 | 直连 |
| `steam-direct.json` | Steam 下载 | 直连 |

## 引用方式

### SRS (推荐)
```json
{
  "tag": "kg-mc",
  "type": "remote",
  "format": "binary",
  "url": "https://github.com/TextlineX/GameRules/releases/download/nightly/kg-mc.srs"
}
```

### JSON (源码)
```json
{
  "tag": "kg-mc",
  "type": "remote",
  "format": "source",
  "url": "https://raw.githubusercontent.com/TextlineX/GameRules/main/src/kg-mc.json"
}
```

## 发布流程

```bash
git add .
git commit -m "update rules"
git tag v1.0.0
git push origin main --tags
```

## ⚠️ 已迁移

**GameRules 已合并到 [DailyRules](https://github.com/TextlineX/DailyRules)**

新的规则文件位置：`DailyRules/src/game/`

本仓库保留仅作历史参考。
