# 闲鱼互动课件上架 Skill

把互动教学 HTML 制作成可核验的闲鱼商品：检查源文件、写真实卖点、设计封面、通过已登录网页发布或替换商品，并打开最终链接验收。

## 在腾讯 WorkBuddy 中安装

下载 [WorkBuddy 导入包](workbuddy-upload.zip)，在 WorkBuddy 左侧“专家·技能·连接器”进入技能页，选择“添加技能 → 上传技能”，选中 ZIP。导入后到“已安装”确认技能已启用；在新对话里说“使用闲鱼互动课件上架技能”。WorkBuddy 的[官方技能说明](https://www.workbuddy.cn/docs/workbuddy/From-Beginner-to-Expert-Guide/Function-Description/Skills-Market)列出了此导入与启用入口。

发布商品前，到“设置 → 智能体 → 浏览器操控”确认浏览器组件可用，并在 WorkBuddy 将要使用的浏览器中登录闲鱼。内置浏览器与 Chrome 等独立浏览器的登录态应分别核对。详见 [WorkBuddy 专用说明](references/workbuddy.md)。

## 在 Codex 中安装

将本仓库文件夹放入 Codex 的 `~/.codex/skills/goofish-courseware-publisher/`，确保 `SKILL.md` 位于该目录根部。重启或刷新 Codex 的技能列表后可用。

## 使用

例如：`使用 $goofish-courseware-publisher，把这份 HTML 课件整理成闲鱼图文，先给我看成品。`

若需要实际上架，请在当次对话明确授权所操作的商品，并在浏览器中自行登录闲鱼。技能不会提供登录凭据，也不会将原始课件、账户资料或商品 ID 上传到此仓库。

封面采用现代明亮的 Rubber-Hose 插画方向，可按当次需求调整；本流程不使用 Runway。批量任务附有[进度记录模板](templates/listing-ledger.csv)。具体工作规则见 [SKILL.md](SKILL.md)。
