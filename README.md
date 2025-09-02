<div align="center">
<img style="width:70%" src="https://count.getloli.com/@astrbot-plugin-choulaopo?name=astrbot-plugin-choulaopo&theme=gelbooru&padding=5&offset=0&align=top&scale=1&pixelated=1&darkmode=auto" alt=":name">

# 随机抽老婆插件 v2.0.4
一个简单的 AstrBot 插件，允许群组成员每天随机抽取另一位群友作为他们的“今日老婆”。v2.0.0 版本经过了完全的重构，优化了代码结构，提升了运行效率和稳定性，并为未来的功能扩展打下了坚实的基础。


[![GitHub](https://img.shields.io/badge/GitHub-astrbot--plugin--choulaopo-blue?style=flat-square&logo=github)](https://github.com/astrbot-plugin-choulaopo)
[![License](https://img.shields.io/github/license/nuomicici/astrbot-plugin-choulaopo?style=flat-square)](https://github.com/nuomicici/astrbot-plugin-choulaopo/blob/main/LICENSE)  
[QQ群](https://qm.qq.com/q/r20HdxCvBe)忘了该怎么写那个卡片了将就着用吧，有bug啥的都可以来
</div>


---
## 2.0.5 更新日志
1. 更新文件名没被记录，现在下载之后那个配置文件名字还是错的，烦的嘞……

## 2.0.4 更新日志
1. 优化了“抽老婆帮助”命令回复的视觉效果

## 2.0.3 更新日志
1. 修复了显示错误的问题。
2. 修复了部分用户不知道为啥出现的某些报错问题，安装如果出现问题，还请等待云数据更新后再更新。

##  2.0.2 更新日志
1. 修复了一点小bug，优化了插件指令判定。

## ✨ v2.0.0 版本更新日志

**本次更新为一次彻底的重构，旨在提升插件的长期可维护性和用户体验。**

-   **🚀 核心逻辑重构**: 完全重写了底层代码，优化了数据处理和事件响应流程，使得插件运行更加稳定和高效。
-   **🔧 配置系统优化**: 添加了配置文件，可以通过配置文件修改每日抽取上限。
-   **💾 数据持久化改进**: 优化了记录的读写机制，避免了重装出现的数据丢失，并确保数据安全。（路径在random_wife，和插件文件夹在同一目录下）。
-   **🧩 代码结构清晰化**: 遵循更严格的模块化设计，将不同功能解耦，便于二次开发和维护。
-   **🐛 错误处理增强**: 添加了更全面的异常捕获和日志记录，帮助管理员快速定位和解决问题。
-   **📄 文档与注释**: 更新了代码注释和此份说明文档，使其更易于理解和使用。

## 🎯 主要功能

-   **每日抽老婆**: 从群聊成员中随机选择一位成为你的“老婆”。
-   **头像展示**: 自动获取并发送被抽中成员的QQ头像。
-   **次数限制**: 可自由配置每人每日的抽取次数。
-   **智能排除**: 自动排除机器人自身、抽取者以及配置文件中指定的黑名单用户。
-   **@功能可选**: 提供带 `@` 和不带 `@` 的两种抽取模式。
-   **历史记录**: 查看你今天抽到的所有“老婆”列表。
-   **数据持久化**: 抽取记录会自动保存在本地，机器人重启不影响。
-   **管理员工具**: 管理员可以随时重置当天的所有抽取记录。
-   **帮助菜单**: 内置详细的帮助说明，方便用户快速上手。

## ⚙️ 安装与配置

### 安装

1. 在插件市场搜索“抽老婆”或“糯米茨”即可安装
2. 或者可以直接克隆源码到插件文件夹：
```
cd /AstrBot/data/plugins
git clone https://github.com/nuomicici/astrbot-plugin-choulaopo/
# 控制台重启AstrBot
```

### 配置

支持面板配置了。

## 📖 命令列表

| 命令 (支持多种别名) | 功能描述 | 备注 |
| :--- | :--- | :--- |
| `今日老婆` / `抽老婆` | 抽取一位群友作为老婆，结果会附带头像并 `@` 该成员。 | |
| `抽老婆-@` / `今日老婆-@` | 功能同上，但结果不会 `@` 该成员，只显示昵称。 | |
| `我的老婆` / `抽取历史` | 查看你今天抽到的所有老婆的历史记录和剩余次数。 | |
| `重置记录` | **[管理员]** 清空服务器上今天所有的抽取记录。 | 需要bot管理员权限 |
| `抽老婆帮助` / `老婆插件帮助` | 显示插件的帮助信息、命令列表和当前配置。 | |

## 📦 依赖

本插件目前仅为 `aiocqhttp` 平台设计和测试，其他平台可能无法正常获取群成员列表。

## 💾 数据存储

插件的数据（每日抽取记录）存储在 `data/plugins/random_wife/wife_records.json` 文件中。每日记录会在第二天第一次触发插件时自动重置。

## 📜 开源许可

本插件使用 [MIT License](https://opensource.org/licenses/MIT) 开源。

## [帮助文档](https://docs.astrbot.app/)
