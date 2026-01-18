# 奶龙 @ 三角洲行动记录平台 (Delta Action Tracker)

![License](https://img.shields.io/badge/License-MIT-blue.svg)
![Platform](https://img.shields.io/badge/Platform-Web-orange.svg)
![Style](https://img.shields.io/badge/UI-iOS26%20Liquid%20Glass-lightblue.svg)

这是一款专为《三角洲行动》玩家打造的个人行动数据记录与可视化平台。采用 **iOS 26 液态玻璃 (Liquid Glass)** 视觉系统设计，支持云端异步存储与多维度收益分析。

## ✨ 核心特性

- 🎨 **前卫视觉设计**：深度模拟 iOS 系统的毛玻璃（Backdrop Filter）、液态流动动效及物理反馈，提供极致的审美体验。
- 📊 **多维度数据分析**：
  - **撤离成功率**：环形闭环可视化展示。
  - **最佳地图识别**：自动计算历史收益最高的作战区域。
  - **收益趋势图**：基于 Chart.js 的贝塞尔曲线，动态展示近 10 场行动的价值波动。
- ☁️ **云端实时同步**：接入 Supabase Serverless 后端，记录永不丢失。
- 📱 **响应式布局**：完美适配 iPhone 灵动岛及各类移动端设备，支持安全区域适配。

## 🛠️ 技术栈

- **Frontend**: HTML5, CSS3 (Advanced Effects), JavaScript (ES6+)
- **Charts**: [Chart.js](https://www.chartjs.org/)
- **Database**: [Supabase](https://supabase.com/) (PostgreSQL)
- **UI Design**: Apple Design Resources 风格延伸

## 🚀 快速开始

### 1. 数据库配置
本项目使用 Supabase 存储数据，你需要创建一个表：
- **表名**: `delta_logs`
- **字段配置**:
  - `id`: int8 (Primary Key)
  - `created_at`: timestamptz (Default: now())
  - `mission_name`: text
  - `operator`: text
  - `result`: text
  - `loot_value`: int8
  - `notes`: text

### 2. 本地运行
1. 克隆仓库：
   ```bash
   git clone [https://github.com/你的用户名/仓库名.git](https://github.com/你的用户名/仓库名.git)
