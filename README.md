# VexOptimizator
Minecraft spigot papermc optimization java plugin .
# VexOptimizator

[![Version](https://img.shields.io/badge/version-1.0.0-blue.svg)](https://github.com/VexTeam/VexOptimizator)
[![Minecraft](https://img.shields.io/badge/Minecraft-1.21-green.svg)](https://papermc.io/)
[![Java](https://img.shields.io/badge/Java-21-orange.svg)](https://adoptium.net/)

An invisible, high-performance optimization engine for Paper servers featuring Smart ClearLag, advanced entity management, and comprehensive server monitoring.

##  Description

VexOptimizator is a powerful, lightweight optimization plugin designed for Minecraft Paper servers. It provides invisible performance enhancements through intelligent monitoring and automatic optimization, featuring a sophisticated Smart ClearLag system that protects player items while maintaining optimal server performance.

The plugin operates seamlessly in the background, dynamically adjusting optimizations based on server load and TPS, ensuring maximum performance without manual intervention.

##  Main Features

###  Core Optimization Modules
- **Smart ClearLag**: Intelligent item cleanup with player protection and configurable intervals
- **Entity Limiter**: Advanced mob spawning control to prevent entity overload
- **Hopper Optimizer**: Efficient hopper network optimization to reduce lag
- **Redstone Profiler**: Complex redstone circuit monitoring and optimization
- **Chunk Cache Cleaner**: Automatic cleanup of unused chunks to free memory
- **Tick Balancer**: Dynamic TPS balancing with automatic optimization triggers

###  Protection & Monitoring
- **Memory Watchdog**: Advanced memory monitoring with emergency measures
- **AFK Optimization**: Reduced view distance for inactive players
- **Module Recovery**: Automatic error handling and module restart capabilities
- **TPS Monitoring**: Real-time performance tracking with diagnostic tools

###  Advanced Features
- **VexAPI Integration**: Seamless integration with VexAPI for enhanced monitoring
- **Async Chunk I/O**: Improved chunk loading/saving performance
- **Entity AI Disable**: Performance boost for entities in unloaded chunks
- **Configurable Warnings**: Customizable countdown messages for ClearLag

##  Installation

### Requirements
- **Minecraft Version**: 1.21+
- **Server Software**: Paper (recommended) or compatible forks
- **Java Version**: 21+
- **Dependencies**: None (VexAPI optional for enhanced features)

### Installation Steps

1. **Download the plugin**
   ```bash
   # Download VexOptimizator-1.0.0.jar from releases
   ```

2. **Place in plugins folder**
   ```bash
   # Copy the jar file to your server's plugins directory
   cp VexOptimizator-1.0.0.jar /path/to/server/plugins/
   ```

3. **Restart your server**
   ```bash
   # The plugin will automatically generate configuration files
   ```

4. **Configure (Optional)**
   - Edit `plugins/VexOptimizator/config.yml` to customize settings
   - Restart server or use `/vexopt reload` to apply changes

### Optional: VexAPI Integration

For enhanced monitoring and statistics:
1. Install VexAPI plugin alongside VexOptimizator
2. Enable integration in `config.yml`:
   ```yaml
   integration:
     vexapi: true
   ```

##  Commands

### Main Command: `/vexopt`
*Permission: `vexopt.admin`*

| Command | Description |
|---------|-------------|
| `/vexopt status` | Show current server optimization status |
| `/vexopt stats` | Display live optimization metrics |
| `/vexopt tps` | Show TPS diagnostics and potential lag sources |
| `/vexopt clear items` | Force immediate item cleanup |
| `/vexopt reload` | Reload configuration without restart |

### ClearLag Command: `/clearlag`
*Permission: `vexopt.clearlag`*

| Command | Description |
|---------|-------------|
| `/clearlag now` | Force immediate item cleanup |
| `/clearlag status` | Show ClearLag module status |
| `/clearlag toggle` | Enable/disable ClearLag (admin only) |

##  Configuration

VexOptimizator includes a comprehensive configuration file (`config.yml`) with detailed explanations for all settings.

### Key Configuration Sections

#### General Optimization Settings
```yaml
general:
  tps_monitor: true          # Enable TPS monitoring
  optimize_entities: true    # Entity optimization
  optimize_redstone: true    # Redstone circuit optimization
  optimize_chunks: true      # Chunk management
  async_chunk_io: true       # Asynchronous chunk operations
```

#### ClearLag Configuration
```yaml
clearlag:
  enabled: true              # Enable automatic cleanup
  interval_minutes: 20       # Cleanup interval
  delete_batch_size: 200     # Items per tick
  player_protect_seconds: 60 # Player item protection time
  warnings: ["10m","5m","4m","3m","2m","1m","20s","10s","5s","4s","3s","2s","1s"]
```

#### Memory Management
```yaml
memory_watchdog:
  enabled: true
  warn_threshold: 0.9        # Warning at 90% memory usage
  emergency_threshold: 0.95  # Emergency measures at 95%
  auto_suspend_tasks: true   # Suspend non-essential tasks
```

#### Module Control
```yaml
modules:
  HopperOptimizer: true
  EntityLimiter: true
  ClearLag: true
```

### Message Customization

All messages can be customized in the configuration file with support for color codes and placeholders:

```yaml
messages:
  prefix: "&b┃ ᴠᴇx&fᴏᴘᴛɪᴍɪᴢᴀᴛᴏʀ &8┃&r "
  clear_complete: "%prefix%&aCleared &f%count% &aitems in &f%time%ms&a."
```

##  Integration

### VexAPI Integration

VexOptimizator seamlessly integrates with VexAPI for enhanced monitoring:

- **Advanced Statistics**: Detailed performance metrics
- **Remote Monitoring**: Server status via external APIs
- **Custom Dashboards**: Integration with monitoring panels

Enable in configuration:
```yaml
integration:
  vexapi: true
  log-level: minimal  # minimal/reduced/full
```

### Plugin Compatibility

- **Compatible**: Works alongside most optimization plugins
- **Smart Detection**: Automatically disables conflicting ClearLag plugins
- **Load Order**: Specify `loadbefore: [VexAPI]` in plugin.yml for proper integration

##  Performance Metrics

Monitor your server's performance with built-in commands:

```
/vexopt stats
```
Shows: TPS, Active Chunks, Entity Count, Memory Usage, Next ClearLag

```
/vexopt tps
```
Provides: TPS diagnostics, memory usage, entity counts, and lag source detection

##  Support

### Getting Help

- **Documentation**: Check the configuration file comments for detailed explanations
- **Commands**: Use `/vexopt status` and `/vexopt tps` for diagnostics
- **Logs**: Check server logs for detailed error information

### Reporting Issues

- **GitHub Issues**: [Create an issue](https://github.com/VexTeam/VexOptimizator/issues) with:
  - Server version and Java version
  - Full server log (during issue)
  - Configuration file
  - Steps to reproduce

### Community Support

- **Discord**: Join our community Discord for real-time support
- **GitHub Discussions**: Community discussions and troubleshooting

##  License

VexOptimizator is licensed under the MIT License. See [LICENSE](LICENSE) file for details.

---

**VexTeam** - High-performance Minecraft server optimizatio
