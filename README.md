# VexOptimizator

A high-performance optimization plugin for Paper servers that improves TPS stability, manages memory, and performs intelligent lag reduction. Operates invisibly and dynamically adjusts optimizations based on load.

## Description

VexOptimizator enhances server performance with Smart ClearLag, entity control, memory management, and TPS monitoring. It runs automatically, requiring no manual tuning.

## Features

Core modules:  
Smart ClearLag – Intelligent cleanup that protects player items  
Entity Limiter – Prevents excessive mob spawning  
Hopper Optimizer – Reduces hopper network lag  
Redstone Profiler – Detects heavy redstone circuits  
Chunk Cache Cleaner – Frees memory from unused chunks  
Tick Balancer – Dynamically maintains TPS  

Protection and monitoring:  
Memory Watchdog – Alerts and recovers on high memory  
AFK Optimization – Reduces load from inactive players  
Module Recovery – Auto restarts failed modules  
TPS Monitor – Real-time diagnostics  

Advanced options:  
VexAPI integration for extended monitoring  
Asynchronous chunk operations  
Entity AI disable for unloaded areas  
Configurable countdowns and messages  

## Installation

Requirements:  
- Minecraft 1.21+  
- Paper server (recommended)  
- Java 21+  
- Optional: VexAPI  

Steps:  
1. Download VexOptimizator.jar from Releases  
2. Place it in `/plugins/`  
3. Restart the server  
4. Edit `config.yml` as needed  
5. Run `/vexopt reload` to apply changes  

## Commands

`/vexopt status` – Show current optimization status  
`/vexopt stats` – Display live metrics  
`/# VexOptimizator

A high-performance optimization plugin for Paper servers that improves TPS stability, manages memory, and performs intelligent lag reduction. Operates invisibly and dynamically adjusts optimizations based on load.

## Description

VexOptimizator enhances server performance with Smart ClearLag, entity control, memory management, and TPS monitoring. It runs automatically, requiring no manual tuning.

## Features

Core modules:  
Smart ClearLag – Intelligent cleanup that protects player items  
Entity Limiter – Prevents excessive mob spawning  
Hopper Optimizer – Reduces hopper network lag  
Redstone Profiler – Detects heavy redstone circuits  
Chunk Cache Cleaner – Frees memory from unused chunks  
Tick Balancer – Dynamically maintains TPS  

Protection and monitoring:  
Memory Watchdog – Alerts and recovers on high memory  
AFK Optimization – Reduces load from inactive players  
Module Recovery – Auto restarts failed modules  
TPS Monitor – Real-time diagnostics  

Advanced options:  
VexAPI integration for extended monitoring  
Asynchronous chunk operations  
Entity AI disable for unloaded areas  
Configurable countdowns and messages  

## Installation

Requirements:  
- Minecraft 1.21+  
- Paper server (recommended)  
- Java 21+  
- Optional: VexAPI  

Steps:  
1. Download VexOptimizator.jar from Releases  
2. Place it in `/plugins/`  
3. Restart the server  
4. Edit `config.yml` as needed  
5. Run `/vexopt reload` to apply changes  

## Commands

`/vexopt status` – Show current optimization status  
`/vexopt stats` – Display live metrics  
`/vexopt tps` – Show TPS and lag sources  
`/vexopt clear items` – Force cleanup  
`/vexopt reload` – Reload configuration  
`/clearlag now` – Manual cleanup  
`/clearlag toggle` – Enable or disable ClearLag  

## Configuration

Example config:
```yaml
general:
  tps_monitor: true
  optimize_entities: true
  optimize_redstone: true
  async_chunk_io: true

clearlag:
  enabled: true
  interval_minutes: 20
  player_protect_seconds: 60
  warnings: ["10m", "5m", "1m", "10s", "5s"]

memory_watchdog:
  enabled: true
  warn_threshold: 0.9
  emergency_threshold: 0.95
 tps` – Show TPS and lag sources  
`/vexopt clear items` – Force cleanup  
`/vexopt reload` – Reload configuration  
`/clearlag now` – Manual cleanup  
`/clearlag toggle` – Enable or disable ClearLag  

## Configuration

Example config:
```yaml
general:
  tps_monitor: true
  optimize_entities: true
  optimize_redstone: true
  async_chunk_io: true

clearlag:
  enabled: true
  interval_minutes: 20
  player_protect_seconds: 60
  warnings: ["10m", "5m", "1m", "10s", "5s"]

memory_watchdog:
  enabled: true
  warn_threshold: 0.9
  emergency_threshold: 0.95

