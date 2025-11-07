# VexOptimizator

Version 1.0.0  
Minecraft 1.21  
Java 21

An invisible, high-performance optimization engine for Paper servers featuring Smart ClearLag, advanced entity management, and comprehensive server monitoring.

## Description

VexOptimizator is a powerful, lightweight optimization plugin designed for Minecraft Paper servers. It provides invisible performance enhancements through intelligent monitoring and automatic optimization, featuring a sophisticated Smart ClearLag system that protects player items while maintaining optimal server performance.

The plugin operates seamlessly in the background, dynamically adjusting optimizations based on server load and TPS, ensuring maximum performance without manual intervention.

## Features

### Core Optimization Modules
Smart ClearLag: Intelligent item cleanup with player protection and configurable intervals  
Entity Limiter: Advanced mob spawning control to prevent entity overload  
Hopper Optimizer: Efficient hopper network optimization to reduce lag  
Redstone Profiler: Complex redstone circuit monitoring and optimization  
Chunk Cache Cleaner: Automatic cleanup of unused chunks to free memory  
Tick Balancer: Dynamic TPS balancing with automatic optimization triggers

### Protection & Monitoring
Memory Watchdog: Advanced memory monitoring with emergency measures  
AFK Optimization: Reduced view distance for inactive players  
Module Recovery: Automatic error handling and module restart capabilities  
TPS Monitoring: Real-time performance tracking with diagnostic tools

### Advanced Features
VexAPI Integration: Seamless integration with VexAPI for enhanced monitoring  
Async Chunk I/O: Improved chunk loading/saving performance  
Entity AI Disable: Performance boost for entities in unloaded chunks  
Configurable Warnings: Customizable countdown messages for ClearLag

## Installation

### Requirements
Minecraft Version: 1.21+  
Server Software: Paper (recommended) or compatible forks  
Java Version: 21+  
Dependencies: None (VexAPI optional for enhanced features)

### Installation Steps

1. Download the plugin  
   Download VexOptimizator-1.0.0.jar from releases

2. Place in plugins folder  
   Copy the jar file to your server's plugins directory

3. Restart your server  
   The plugin will automatically generate configuration files

4. Configure (Optional)  
   Edit plugins/VexOptimizator/config.yml to customize settings  
   Restart server or use /vexopt reload to apply changes

### Optional: VexAPI Integration

For enhanced monitoring and statistics:  
1. Install VexAPI plugin alongside VexOptimizator  
2. Enable integration in config.yml

## Commands

### Main Command: /vexopt
Permission: vexopt.admin

```
/vexopt status
/vexopt stats
/vexopt tps
/vexopt clear items
/vexopt reload
```

### ClearLag Command: /clearlag
Permission: vexopt.clearlag

```
/clearlag now
/clearlag status
/clearlag toggle
```

## License

VexOptimizator is licensed under the MIT License. See LICENSE file for details.

## Discord
[![Join our Discord](https://img.shields.io/badge/Discord-Join%20Now-5865F2?logo=discord&logoColor=white)](https://discord.gg/EH7afrRCQv)

