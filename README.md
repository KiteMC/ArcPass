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

- **Multi-Tier Pass System** - Free, Premium, VIP tiers with independent reward tracks
- **Rich Quest System** - Daily, weekly, seasonal, and story quests
- **Flexible Rewards** - Items, economy, permissions, titles, cosmetics
- **Multi-Currency** - Vault/CMI economy and points plugins (PlayerPoints, CoinsEngine, TokenManager)
- **Title Plugins** - DeluxeTags, TAB, PlayerTitle, NametagEdit with automatic fallback
- **Season Management** - Complete season control with progress reset
- **Customizable GUI** - Fully configurable interface system
- **Leaderboards** - Level, experience, and season rankings
- **Wide Compatibility** - LuckPerms, PlaceholderAPI, MythicMobs, Jobs, and more
- **Folia Support** - Full multi-threaded server compatibility

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

- **Discord**: [Join our community](https://discord.com/invite/TCn9v88V)
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
    compileOnly("com.kitemc:arcpass-api:1.2.2")
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
    <version>1.2.2</version>
    <scope>provided</scope>
</dependency>
```

---

<div align="center">

**Made with ❤️ by [KiteMC](https://github.com/KiteMC)**

</div>
