<div align="center">

# ArcPass

**A powerful Battle Pass plugin for Minecraft servers**

[![Latest Release](https://img.shields.io/github/v/release/KiteMC/ArcPass?style=flat-square&label=Latest)](https://github.com/KiteMC/ArcPass/releases/latest)
[![Downloads](https://img.shields.io/github/downloads/KiteMC/ArcPass/total?style=flat-square)](https://github.com/KiteMC/ArcPass/releases)
[![License](https://img.shields.io/badge/License-Proprietary-red?style=flat-square)](https://license.kitemc.com/products/arcpass)

[Documentation](https://kitemc.com/docs/arcpass/) • [Purchase](https://license.kitemc.com/products/arcpass) • [Discord](https://discord.com/invite/TCn9v88V)

</div>

---

## About

ArcPass is a premium Battle Pass plugin that brings seasonal progression, quests, and rewards to your Minecraft server. Create engaging gameplay experiences with multi-tier passes, diverse quest types, and flexible reward systems.

## Features

- **Passes & Seasons** - Multiple independent passes, free/paid tiers, season lifecycle management, archiving, and progress resets.
- **Quests & Progression** - Daily, weekly, seasonal, challenge, and story quests, including per-minute `playtime` progression.
- **Rewards & Integrations** - Item, command, economy, permission, title, and particle rewards with support for Vault/CMI, PlayerPoints, LuckPerms, PlaceholderAPI, and more.
- **GUI & Localization** - YAML-driven GUI, RGB colors, ItemsAdder/Oraxen icons, multilingual configuration, and hot reload.
- **Server & Storage** - Folia support, SQLite/MySQL/MariaDB storage, and cross-server synchronization through shared databases or Redis.
- **Administration & API** - Level/experience leaderboards, autosave with retry handling, and a developer API.

## Requirements

- **Server**: Paper, Spigot, Bukkit, or Folia (1.18 - 1.21+)
- **Java**: 17 or higher (21 recommended)
- **License**: Valid ArcPass license required

## Installation

1. Download the latest `ArcPass-x.x.x.jar` from [Releases](https://github.com/KiteMC/ArcPass/releases/latest)
2. Place the JAR in your server's `plugins` folder
3. Start the server to generate config files
4. Configure your license key in `plugins/ArcPass/license.yml`
5. Restart the server

## License

ArcPass is a paid plugin. Licenses are available through Alipay and USDT channels, and a valid license is required for full functionality.

| Plan         | Alipay Price | USDT Price | Scope |
|--------------|--------------|------------|-------|
| Standard     | CNY 68       | USD 12.99  | Basic single-server battle pass features |
| Professional | CNY 198      | USD 29.99  | Multi-server deployment, cross-server sync, Developer API, and priority support |

**[Purchase License](https://license.kitemc.com/products/arcpass)**

### Plan Comparison

| Feature                          | Standard | Professional |
|----------------------------------|:--------:|:------------:|
| Multi-Pass System                | ✅       | ✅           |
| Multi-Tier Rewards               | ✅       | ✅           |
| Quest System (All Types)         | ✅       | ✅           |
| Season Management                | ✅       | ✅           |
| Leaderboards                     | ✅       | ✅           |
| Database (SQLite / MySQL)        | ✅       | ✅           |
| Cross-Server (Redis / Shared DB) | ❌       | ✅           |
| Folia Support                    | ✅       | ✅           |
| PlaceholderAPI / Integrations    | ✅       | ✅           |
| Multi-Language (i18n)            | ✅       | ✅           |
| Customizable GUI                 | ✅       | ✅           |
| Hot Reload                       | ✅       | ✅           |
| Lifetime Updates                 | ✅       | ✅           |
| **Developer API**                | ❌       | ✅           |
| Priority Support                 | ❌       | ✅           |

## Documentation

- [Getting Started](https://kitemc.com/docs/arcpass/guide/)
- [Configuration](https://kitemc.com/docs/arcpass/config/)
- [Developer API](https://kitemc.com/docs/arcpass/developer/)
- [FAQ](https://kitemc.com/docs/arcpass/faq/)

## Support

- **Discord**: [Join our community](https://discord.gg/dcsBw5Z5ZT)
- **Email**: <starry_cbz@outlook.com>
- **License Center**: [Manage your licenses](https://license.kitemc.com/dashboard/licenses)

## Developer API

ArcPass provides a comprehensive API for developers. See the [API documentation](https://kitemc.com/docs/arcpass/developer/) for details.

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

---

<div align="center">

**Made with ❤️ by [KiteMC](https://github.com/KiteMC)**

</div>
