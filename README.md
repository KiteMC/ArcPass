[English README](README_en.md)

# ArcPass

<div align="center">

![版本](https://img.shields.io/badge/版本-1.9.2-blue)
![Minecraft](https://img.shields.io/badge/Minecraft-1.18--1.21+-green)
![Java](https://img.shields.io/badge/Java-17+-orange)
![平台](https://img.shields.io/badge/平台-Paper%20%7C%20Spigot%20%7C%20Folia-purple)

**现代化的 Minecraft 服务器战斗通行证系统**

[English](README_en.md) | [文档](https://kitemc.com/zh/docs/arcpass/) | [Discord](https://discord.com/invite/TCn9v88V)

</div>

---

## 功能特性

- 🎮 **通行证与赛季** - 支持多个独立通行证、免费/付费档位、赛季生命周期管理、进度归档与重置。
- 🎯 **任务与进度** - 支持日常、周常、赛季、挑战和剧情任务，也可按在线分钟累计 `playtime` 进度。
- 🎁 **奖励与集成** - 支持物品、命令、经济、权限、称号和粒子奖励；兼容 Vault/CMI、PlayerPoints、LuckPerms、PlaceholderAPI 等插件。
- 🖥️ **界面与本地化** - YAML 可配置 GUI、RGB 颜色、ItemsAdder/Oraxen 图标和多语言配置，支持热重载。
- 🌐 **服务器与数据** - 支持 Folia、SQLite、MySQL/MariaDB，以及共享数据库或 Redis 跨服同步。
- 📊 **管理与开发** - 提供等级/经验排行榜、自动保存、失败重试和开发者 API。

## 环境要求

- Java 17 或更高版本
- Paper/Spigot 1.18+ 或 Folia 1.20+
- (可选) Vault / CMI - 经济系统集成
- (可选) PlayerPoints / CoinsEngine / TokenManager - 点卷货币
- (可选) PlaceholderAPI - 变量支持
- (可选) LuckPerms - 权限奖励
- (可选) DeluxeTags / TAB / PlayerTitle / NametagEdit - 称号奖励
- (可选) PlayerParticles - 装饰粒子奖励

## 安装方法

1. 从 [Releases](https://github.com/KiteMC/ArcPass/releases/latest) 下载 `ArcPass.jar`
2. 将文件放入服务器的 `plugins` 文件夹
3. 重启服务器
4. 在 `plugins/ArcPass/` 中配置插件
5. 在 `license.yml` 中填入您的许可证密钥

## 命令列表

| 命令 | 描述 | 权限 |
|------|------|------|
| `/ap` | 打开主菜单 | `arcpass.use` |
| `/ap level` | 查看当前等级 | `arcpass.command.level` |
| `/ap quests` | 查看任务 | `arcpass.command.quests` |
| `/ap claim` | 领取奖励 | `arcpass.command.claim` |
| `/ap admin` | 管理员面板 | `arcpass.admin` |

## 配置文件

<details>
<summary>config.yml</summary>

```yaml
# 默认语言
locale:
  default: zh_CN

# 通行证设置
pass:
  max-level: 100
  base-experience: 100
  experience-multiplier: 1.1

# 调试模式
debug: false
```

</details>

## 开发者 API

### Gradle (Kotlin DSL)

```kotlin
repositories {
    maven("https://maven.pkg.github.com/KiteMC/ArcPass")
}

dependencies {
    compileOnly("com.kitemc:arcpass-api:1.9.2")
}
```

### Maven

```xml
<repository>
    <id>github</id>
    <url>https://maven.pkg.github.com/KiteMC/ArcPass</url>
</repository>

<dependency>
    <groupId>com.kitemc</groupId>
    <artifactId>arcpass-api</artifactId>
    <version>1.9.2</version>
    <scope>provided</scope>
</dependency>
```

### 使用示例

```java
import com.kitemc.arcpass.api.ArcPassAPI;
import com.kitemc.arcpass.api.ArcPassProvider;

public class MyPlugin extends JavaPlugin {

    @Override
    public void onEnable() {
        // 检查 ArcPass 是否已加载
        if (ArcPassProvider.isLoaded()) {
            ArcPassAPI api = ArcPassProvider.get();

            // 获取玩家数据
            api.getPlayerData(player.getUniqueId())
                .thenAccept(data -> {
                    data.ifPresent(playerData -> {
                        int level = playerData.getLevel();
                        getLogger().info("玩家等级: " + level);
                    });
                });

            // 添加经验
            api.addExperience(player.getUniqueId(), 100);
        }
    }
}
```

### 事件监听

```java
@EventHandler
public void onLevelUp(PlayerLevelUpEvent event) {
    Player player = Bukkit.getPlayer(event.getPlayerId());
    if (player != null) {
        player.sendMessage("恭喜！您已达到 " + event.getNewLevel() + " 级");
    }
}
```

## 变量 (PlaceholderAPI)

需要安装 PlaceholderAPI。

| 变量 | 描述 |
|------|------|
| `%arcpass_level%` | 当前等级 |
| `%arcpass_exp%` | 总经验值 |
| `%arcpass_exp_next%` | 升级所需经验 |
| `%arcpass_rank_level%` | 等级排行榜排名 |
| `%arcpass_rank_exp%` | 经验排行榜排名 |

## 技术支持

- 📖 [在线文档](https://kitemc.com/zh/docs/arcpass/)
- 💬 [Discord](https://discord.com/invite/TCn9v88V)
- 📧 邮箱: <starry_cbz@outlook.com>

## 许可协议

本插件为付费插件，禁止未经授权的传播。支持支付宝和 USDT 渠道购买许可证。

| 版本 | 支付宝价格 | USDT 价格 | 适用场景 |
|------|------------|-----------|----------|
| 标准版 | 68 元 | 10.99 USD | 单服基础通行证功能 |
| 专业版 | 198 元 | 29.99 USD | 多服部署、跨服同步、开发者 API 与优先支持 |

购买许可证：[KiteMC License Platform](https://license.kitemc.com/products/arcpass)

© 2024-2026 KiteMC. 保留所有权利。
