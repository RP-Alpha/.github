# RP-Alpha

<div align="center">
  <h3>Modern, Open-Source FiveM Resources</h3>
  <p>Compatible with <strong>QB-Core</strong> | <strong>QBOX</strong> | <strong>OX_CORE</strong></p>
</div>

---

## 📦 Available Resources

| Resource | Description | Status |
|----------|-------------|--------|
| **[rpa-lib](https://github.com/RP-Alpha/rpa-lib)** | Core library & framework bridge (Required) | ✅ Stable |
| **[rpa-notify](https://github.com/RP-Alpha/rpa-notify)** | Modern glassmorphism notifications | ✅ Stable |
| **[rpa-textui](https://github.com/RP-Alpha/rpa-textui)** | Clean interaction prompts | ✅ Stable |
| **[rpa-blips](https://github.com/RP-Alpha/rpa-blips)** | Config-based map blip manager | ✅ Stable |
| **[rpa-spawn](https://github.com/RP-Alpha/rpa-spawn)** | Spawn selector with skycam | ✅ Stable |
| **[rpa-appearance](https://github.com/RP-Alpha/rpa-appearance)** | Appearance system bridge | ✅ Stable |
| **[rpa-fuel](https://github.com/RP-Alpha/rpa-fuel)** | Target-based fuel system | ✅ Stable |
| **[rpa-banking](https://github.com/RP-Alpha/rpa-banking)** | Modern banking UI | ✅ Stable |
| **[rpa-shops](https://github.com/RP-Alpha/rpa-shops)** | Config-driven shop system | ✅ Stable |
| **[rpa-consumables](https://github.com/RP-Alpha/rpa-consumables)** | Food, drinks, alcohol, smokeables | ✅ Stable |
| **[rpa-garages](https://github.com/RP-Alpha/rpa-garages)** | Vehicle storage & retrieval | ✅ Stable |
| **[rpa-housing](https://github.com/RP-Alpha/rpa-housing)** | Shell-based property system | ✅ Stable |
| **[rpa-vehiclekeys](https://github.com/RP-Alpha/rpa-vehiclekeys)** | Vehicle lock/unlock & engine control | ✅ Stable |
| **[rpa-tuning](https://github.com/RP-Alpha/rpa-tuning)** | Vehicle mod shop with RGB neons | ✅ Stable |
| **[rpa-dispatch](https://github.com/RP-Alpha/rpa-dispatch)** | Emergency dispatch system | ✅ Stable |
| **[rpa-mdt](https://github.com/RP-Alpha/rpa-mdt)** | Mobile Data Terminal | ✅ Stable |
| **[rpa-police](https://github.com/RP-Alpha/rpa-police)** | Police job with evidence system | ✅ Stable |
| **[rpa-ambulance](https://github.com/RP-Alpha/rpa-ambulance)** | EMS job with revive mechanics | ✅ Stable |
| **[rpa-cityhall](https://github.com/RP-Alpha/rpa-cityhall)** | Licenses & government services | ✅ Stable |
| **[rpa-jobs](https://github.com/RP-Alpha/rpa-jobs)** | Civilian jobs with XP system | ✅ Stable |

---

## 🚀 Quick Start

### Prerequisites
- A FiveM server running **QB-Core**, **QBOX**, or **OX_CORE**
- **oxmysql** (recommended)
- **ox_target** or **qb-target** (for interaction prompts)

### Installation

1. **Download** the resources you need from the links above.

2. **Extract** each resource to your server's `resources` folder.

3. **Add to server.cfg** in this order:
   ```cfg
   # Core (REQUIRED FIRST)
   ensure rpa-lib

   # UI Systems
   ensure rpa-notify
   ensure rpa-textui
   ensure rpa-blips

   # Player Systems
   ensure rpa-spawn
   ensure rpa-appearance
   ensure rpa-consumables

   # Economy
   ensure rpa-banking
   ensure rpa-shops
   ensure rpa-fuel

   # Vehicles
   ensure rpa-garages
   ensure rpa-vehiclekeys
   ensure rpa-tuning

   # Properties
   ensure rpa-housing

   # Jobs
   ensure rpa-jobs
   ensure rpa-police
   ensure rpa-ambulance
   ensure rpa-dispatch
   ensure rpa-mdt
   ensure rpa-cityhall
   ```

4. **Configure** each resource via its `config.lua` file.

5. **Restart** your server.

---

## 📥 Full Suite Download

Want everything at once? Download the complete **RP-Alpha Suite** from our [Releases](https://github.com/RP-Alpha/rp-alpha-suite/releases) page.

---

## 🔧 Configuration

Each resource includes a `config.lua` with sensible defaults. Common options:

| Option | Description |
|--------|-------------|
| `Config.Debug` | Enable debug prints |
| `Config.Locale` | Language for notifications (default: `'en'`) |
| `Config.Framework` | Auto-detected, but can be forced |

Refer to individual resource READMEs for specific configuration options.

---

## 🌐 Framework Compatibility

RP-Alpha automatically detects and bridges to your framework:

| Framework | Support Level |
|-----------|---------------|
| QB-Core | ✅ Full |
| QBOX | ✅ Full |
| OX_CORE | ✅ Full |

---

## 🤝 Support

- **Issues**: [GitHub Issues](https://github.com/RP-Alpha/.github/issues)
- **Discord**: Coming Soon

---

## 📄 License

All RP-Alpha resources are released under the **MIT License**. Free to use, modify, and distribute.

---

<div align="center">
  <sub>Built with ❤️ by the RP-Alpha Community</sub>
</div>
