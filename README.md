# agency-experts-workbuddy

WorkBuddy 专家包集合，由 [msitarzewski/agency-agents](https://github.com/msitarzewski/agency-agents)（MIT）转换而来。共 **250 个专家**，覆盖工程研发、数据智能、营销增长、产品设计、安全合规、行业顾问等方向，每个专家含独立 emoji 头像。

## 安装

将本仓库克隆或解压到 WorkBuddy 的「我的专家」市场目录：

- **Windows**：`C:\Users\<用户名>\.workbuddy\plugins\marketplaces\my-experts\`
- **macOS / Linux**：`~/.workbuddy/plugins/marketplaces/my-experts/`

> 如果目标位置已有自己的 `my-experts`，可把本仓库目录改名为 `agency-experts/` 放在同级 `…\plugins\marketplaces\agency-experts\`，与原市场并存。

完全退出并重启 WorkBuddy，左侧「专家」入口刷新即可看到这些专家。

## 推送记录（Push Log / Changelog）

> 本仓库由脚本/智能体持续整理与推送。下方仅记录有实质新增/改写的推送，便于协作者快速了解「推了什么、有什么用」；纯批量格式转写不单独列条。

| 日期 | Commit | 变更内容 | 作用 / 用途 |
|------|--------|----------|------------|
| 2026-08-13 | `e127ef5` | ① 新增 **hallmark** 反 AI 味设计专家完整插件（`plugin.json` + `README.md` + `agents/hallmark.md` + `avatars/expert.png` + **106** 个 `references/` 设计规则文档）；② 顶层专家数 249 → **250**；③ `.codebuddy-plugin/marketplace.json` 登记 hallmark 条目 | **hallmark**：源自 [Nutlope/hallmark](https://github.com/Nutlope/hallmark)（Together AI，MIT）的「反 AI 味」设计规范专家。动词 `build / audit / redesign / study`；58 道 slop 检测闸门 + 21 种宏观结构 + 20 套主题，强制结构多样性，专治 AI 一眼假的紫色渐变+三列卡片套路，提升作品集 / 落地页 / 企业原型的视觉质感。 |
| 2026-08-13 | `e127ef5` | 重写 **wechat-official-account/README.md**（公众号文章助手说明） | **公众号文章助手**：源自 The Agency 公众号运营角色设定。专注公众号内容营销、涨粉与转化优化。核心能力：60/30/10 内容法则、标题封面钩子目标打开率 ≥30%、图文/消息/投票/小程序/菜单多形态组合、自动回复与关键词转化、打开率-点击率-转化率数据分析迭代。 |

> 各专家详细规则与使用示例见对应 `plugins/<专家名>/README.md`。

## 许可

派生自 [agency-agents](https://github.com/msitarzewski/agency-agents)（MIT）。保留原始署名与 MIT 许可，详见 `LICENSE` 与 `NOTICE.md`。
本仓库不构成原创作品集，仅作为第三方智能体定义的格式转换与整理。
