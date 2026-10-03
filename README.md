# ⚒️ SkriptForge

A growing collection of **ready-to-use Skript scripts for Minecraft 1.8.8 servers**.

SkriptForge is focused on one thing: providing practical, clean, easy-to-edit `.sk` scripts that server owners and Skript developers can drop into their projects and customize.

> Community-made resource. Not affiliated with Mojang Studios or Microsoft.

## ✨ What is SkriptForge?

SkriptForge is now a **Skript-only project**.

There are **no bundled JAR files, server binaries, or addon plugins** in this repository. The project contains Skript source files and documentation so you can use the scripts with your own Minecraft server setup.

## 📦 Included Scripts

Current scripts include:

### 👤 Player Utilities

- `/spawn`
- `/setspawn`
- `/sethome`
- `/home`
- `/delhome`
- `/tpa`
- `/tpaccept`
- `/tpdeny`
- `/fly`
- `/hat`
- `/suicide`

### 🛠️ Server Utilities

- `/broadcast`
- `/day`
- `/night`
- `/feed`
- `/heal`
- `/workbench`

### 🌎 Warps

- `/setwarp <name>`
- `/warp <name>`
- `/delwarp <name>`

### 🛡️ Administration

- `/kick`
- `/mute`
- `/unmute`
- Basic muted-chat protection
- Admin permissions for sensitive commands

### 💰 Economy

- `/balance`
- `/bal`
- `/pay`
- `/setmoney`
- Simple player balance storage

### 🎉 Player Events

- First-join welcome messages
- Join messages
- Quit messages

More scripts will be added over time.

## 📁 Project Structure

```text
SkriptForge/
├── scripts/
│   ├── admin.sk
│   ├── economy.sk
│   ├── essentials.sk
│   ├── player-utilities.sk
│   ├── server-utilities.sk
│   ├── spawn.sk
│   ├── tpa.sk
│   └── warps.sk
└── README.md
```

The `.sk` files are the main product of this repository.

## 🚀 Installation

1. Install a Minecraft **1.8.8** server such as your preferred compatible server software.
2. Install a Skript version compatible with your server.
3. Clone or download this repository.
4. Copy the scripts from `scripts/` into:

```text
plugins/Skript/scripts/
```

5. Start your server.
6. Reload the scripts with the appropriate Skript reload command for your installation.

Example:

```text
/sk reload all
```

> The exact Skript command and syntax can vary between Skript versions. Check your installed version if a script reports an error.

## 🎯 Target

| Component | Target |
| --- | --- |
| Minecraft | Java Edition 1.8.8 |
| Project type | Skript library |
| Format | `.sk` |
| Focus | Server utilities & gameplay scripts |
| Bundled JARs | None |
| Server binaries | None |

## ⚠️ Compatibility

SkriptForge is designed around the **Minecraft 1.8.8** ecosystem and conservative Skript syntax.

Because Skript syntax and available expressions can differ between versions, always test scripts on a development server before deploying them to a production server.

Some scripts may require functionality provided by your installed Skript version. This repository intentionally does **not** bundle Skript or third-party addon JARs.

## 🧩 Configuration

Many scripts store their data using Skript variables, for example:

```text
{skriptforge.spawn}
{skriptforge.home.%player%}
{skriptforge.warp.%arg-1%}
```

You can customize messages, permissions, commands, and variable names directly inside the `.sk` files.

## 🔐 Permissions

Scripts use dedicated `skriptforge.*` permissions where appropriate.

Examples:

```text
skriptforge.admin
skriptforge.warp.admin
```

Configure these permissions using your preferred permissions system.

## 🧑‍💻 Development

Want to add a script?

1. Create a new `.sk` file inside `scripts/`.
2. Keep it compatible with Minecraft 1.8.8.
3. Use clear command names and permissions.
4. Avoid unnecessary dependencies.
5. Test it on a clean server.
6. Add the script to this README when appropriate.

## 🤝 Contributing

Contributions are welcome.

Good contributions include:

- New standalone Skript utilities
- Bug fixes
- Compatibility improvements
- Better permissions
- Cleaner messages
- Performance improvements
- Documentation improvements

Please keep scripts simple, readable, and easy for server owners to customize.

## 🗺️ Roadmap

Planned additions include:

- 🛡️ Advanced moderation scripts
- 🖥️ Server management utilities
- 🎁 Kits and daily rewards
- 💰 Expanded economy features
- 🛒 Simple shop systems
- 🎨 GUI-based utilities where possible
- 📊 Player statistics
- 🔒 Protection utilities
- 📢 Announcement systems
- 🧰 More administrator tools

## 📜 Disclaimer

Minecraft is a trademark of Mojang Studios/Microsoft. SkriptForge is an independent community project and is not affiliated with or endorsed by Mojang Studios or Microsoft.

## 📄 License

See the repository's `LICENSE` file for licensing information.

---

⭐ If SkriptForge helps your server, consider starring the repository and contributing new scripts.