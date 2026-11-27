# 在腾讯 WorkBuddy 桌面版中使用

此文件仅用于 WorkBuddy 的运行环境。Workbench/CodeBuddy IDE 是不同产品，不要把它的 `.codebuddy/skills/` 路径套到 WorkBuddy 桌面版。

## 安装与启用

在 WorkBuddy 左侧的“专家·技能·连接器”中进入技能页，用“添加技能 → 上传技能”导入包含本技能文件夹的 ZIP 或文件夹。随后在“已安装”中确认 `goofish-courseware-publisher` 已启用；关闭的技能不会参与新任务。可在对话中明确说“使用闲鱼互动课件上架技能”。

本机若已确认用户级技能目录为 `~/.workbuddy/skills/`，也可将完整技能文件夹放在该目录。复制文件只证明文件落地，**不能代替**在客户端“已安装”列表中核对可发现、已启用。勿覆盖其他同名技能；更新前保留上一版，核验新版后再清理备份。若本轮无法读取 WorkBuddy 客户端状态，如实报告“已部署文件、客户端加载未验收”。

## 选择浏览器和文件

1. WorkBuddy 的内置浏览器首次使用可能需要在“设置 → 智能体 → 浏览器操控”安装组件。Chrome、Edge、QQ 等独立浏览器需安装并连接 WorkBuddy 扩展。先核对当前工具和登录态，再选用户指定或已经登录闲鱼的浏览器；WorkBuddy 内置浏览器、独立浏览器与其他 AI 应用的会话不一定共享登录。
2. 用户在浏览器里自行完成登录、验证码或安全验证。技能不要读取密码、Cookie 或令牌。浏览器控制不可用时先完成本地封面、文案与图片，不要宣称已经上架。
3. 源 HTML 从用户附件或获授权的本地工作空间读取；产物写进当次工作空间。先用浏览器预览或静态检查确认课件功能，再写卖点。不要把原课件或私有工作空间作为公开技能资源。
4. 在闲鱼上传封面与详情图前，检查 WorkBuddy 当前浏览器工具是否能选择本地文件并回读上传状态。若不能，先看当前已获授权且已登录的其他浏览器控制路径是否支持可观察的文件选择；仍不可用时只请用户完成文件选择，随后继续检查表单、发布和成品页。不要调用未验证的私有上传接口，也不要把另一浏览器的登录态视作可复用。

## 批量任务恢复

把 `templates/listing-ledger.csv` 复制到当前工作空间，按课件逐行更新源文件校验值、交付方式和商品状态。`stage` 使用 `pending`、`assets_ready`、`form_filled`、`submitted`、`verified` 或 `old_unlisted`；每次状态变化都保存，尤其在点击发布前后。`submitted` 不是完成状态，重启后应先从卖家列表核查是否已有新商品。最终以 `verified`（新上架）或 `old_unlisted`（替换完成）为准，并附完整商品链接。类目或交付阻塞时在 `notes` 记下页面原文和待核实点，不冒充 `verified`。

不要让模板中的示例值、上一轮记录或 Skill 本身替代当前用户的价格、标题、商品范围与发布授权。

## 可用的官方入口

- [WorkBuddy 技能安装和启用](https://www.workbuddy.cn/docs/workbuddy/From-Beginner-to-Expert-Guide/Function-Description/Skills-Market)
- [WorkBuddy 浏览器操控和登录态](https://cloud.tencent.com/document/product/1831/134400)
