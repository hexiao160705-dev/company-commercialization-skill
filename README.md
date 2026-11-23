# Company Commercialization Skill · 公司商业化技能

Coordinate product, marketing and operations around a business decision. One entry skill routes a request into 32 task cards backed by 206 upstream skills. Each card specifies the inputs, expected handoff and next decision. The [interactive map](商业化任务拓扑.html) shows 244 task-to-skill links. Download and open the HTML locally to explore it.

用一个入口协调产品、市场和职能部门。AI 先确定这次要做的决定，再选择任务卡、核对证据，把结果交给下一位负责人。包内有 32 张中文任务卡、206 个保留原文的上游技能和离线拓扑图。

## Install · 安装

1. Download the named ZIP asset from [Releases](https://github.com/hexiao160705-dev/company-commercialization-skill/releases). Unzip it. 从发布页下载安装包并解压。
2. Copy the entire `company-commercialization` folder into `~/.codex/skills/`. Start a new Codex chat. 将整个同名文件夹复制到该技能目录，开启新对话。
3. Invoke `$company-commercialization` and describe the decision, available evidence and desired result. 也可以直接让支持本地文件的 AI 阅读 [SKILL.md](company-commercialization/SKILL.md)。

## Try it · 使用示例

> $company-commercialization — Six customers are eligible to renew. Three renewed, two declined and one has not replied. Four others are not yet due. Report the confirmed renewal rate and assign the next follow-up.

> 用 $company-commercialization 分析续购。十家客户中六家已到期，其中三家续购、两家退出、一家未回复。请给出分母、截至今天的续购率，并列出下一步由谁跟进。

The renewal card should report 3/6 (50%), keep the pending account visible, and leave the four future renewals outside today's denominator. 第二版另有两张判断卡，分别核对订单能否排期，以及一笔账面盈利的订单在尾款到账前是否需要垫资。

## Contents and scope · 内容与边界

- [Task cards / 任务卡](company-commercialization/references/tasks/) and [source catalog / 来源目录](company-commercialization/references/catalog.json). The catalog pins source revisions and hashes. 目录保留来源版本、许可证和正文指纹。
- Task cards and the interactive map are primarily in Chinese. Many upstream instructions are in English. 这份项目说明提供中英双语。
- External accounts and connectors are optional and must be configured separately. Generated recommendations require evidence from the actual business. 公开包不包含书籍全文或用户业务数据。
- Original project materials are MIT-licensed. Files under references/sources retain their upstream licenses and notices. 本项目原创部分采用 [MIT](LICENSE)，第三方内容遵循各自所附许可。
