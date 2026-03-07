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

- **Multi-Pass System** - Define multiple passes (Combat, Explorer, Builder, etc.) with independent progression
- **Multi-Tier Rewards** - Free, Premium, VIP tiers with independent reward tracks per pass
- **Rich Quest System** - Daily, weekly, seasonal, challenge, and story quests with auto-reset
- **Flexible Rewards** - Items, commands, economy, permissions, titles, cosmetics
- **Multi-Currency** - Vault/CMI economy and points plugins (PlayerPoints, CoinsEngine, TokenManager)
- **Title Plugins** - DeluxeTags, TAB, NametagEdit with automatic fallback chain
- **Season Management** - Complete season lifecycle with archiving and progress reset
- **Customizable GUI** - YAML-driven interface with ItemsAdder & Oraxen icon support
- **Leaderboards** - Level and experience rankings with caching
- **Database Support** - SQLite and MySQL/MariaDB with automatic schema migration
- **Auto-Save** - Configurable periodic saves with dirty-tracking and failure retry
- **Hot Reload** - Reload configs, passes, quests, rewards, and language files without restart
- **Wide Compatibility** - LuckPerms, PlaceholderAPI, MythicMobs, Jobs Reborn, and more
- **Folia Support** - Full region-based scheduling compatibility
- **Multi-Language** - Built-in i18n with per-player locale support

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

ArcPass is a paid plugin. A valid license is required for full functionality.

| Plan         | Price  | Devices | Ports/Device | Extras                             |
|--------------|--------|---------|--------------|-------------------------------------|
| Standard     | $12.99 | 5       | 3            | Lifetime updates                    |
| Professional | $29.99 | 25      | 15           | Lifetime updates, Priority support  |

**[Purchase License](https://license.kitemc.com/products/arcpass)**

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
    compileOnly("com.kitemc:arcpass-api:1.3.3")
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
    <version>1.3.3</version>
    <scope>provided</scope>
</dependency>
```

---

<div align="center">

**Made with ❤️ by [KiteMC](https://github.com/KiteMC)**

</div>
