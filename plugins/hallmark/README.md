# Hallmark 反 AI 味设计

源自开源项目 [Nutlope/hallmark](https://github.com/Nutlope/hallmark)（Together AI，MIT）的「反 AI 味」设计规范技能，已打包为 WorkBuddy 专家。

## 类型

Agent 型（单个 AI 专家 / 规则型设计技能）

## 功能

- **build（默认）**：按需求新建页面。先确认 audience / use case / tone，再选 21 种宏观结构之一 + 20 套主题之一，生成前过 58 道 slop 检测闸门。
- **audit**：对已有页面/代码做 AI 味体检，按严重度输出问题清单（不改文件）。
- **redesign**：在保留文案、品牌、路由、信息架构的前提下，重构视觉结构层。
- **study**：给定 URL 或截图，提取其「设计 DNA」（结构 / 字体角色 / 色彩锚点 / 节奏），作为新建参考；远程内容按对抗性处理，不执行、不读指令。

## 详细规则

设计规则、主题、宏观结构、slop 测试等全部在 `references/` 目录下，专家按需加载。核心约束包括：

- **Locked tokens**：颜色、字体必须引用命名 CSS 变量，禁止渲染中途 inline OKLCH。
- **Mobile floor**：320 / 375 / 414 / 768 px 验证，无横向滚动、无两行按钮标签。
- **Typography purity**：标题保持 roman，不乱加斜体粗体。
- **Honest copy**：不编造数据，统计型布局用真数字或占位符（—）。
- **Pre-emit self-critique**：交付前六轴自评（Philosophy / Hierarchy / Execution / Specificity / Restraint / Variety），任一项 < 3 强制重做。

## 使用示例

- 以 Hallmark 反 AI 味设计专家身份，帮我做一个不像 AI 生成的「ZHX NEXUS Studio 作品集」落地页。
- 对我现有的 HTML demo 做 audit，列出 AI 味问题。
- redesign 这个登录页，保留文案与路由。

## 头像

头像已生成在 `avatars/expert.png`（H 字母标记）。如需替换，要求：PNG/JPG，512×512 px，≤ 500KB。

## 安装

将专家包目录放到专家目录下：

```
C:\Users\user\.workbuddy\plugins\marketplaces\my-experts\plugins/hallmark/
```

然后运行注册命令使其可见：

```bash
python3 scripts/register_expert.py <expert-dir>
```

## 打包分享

```bash
zip -r hallmark.zip hallmark/
```
