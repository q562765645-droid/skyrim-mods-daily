# USER.md - About Your Human

_Learn about the person you're helping. Update this as you go._

- **Name:**
- **What to call them:**
- **Pronouns:** _(optional)_
- **Timezone:**
- **Notes:**

## Context

_(What do they care about? What projects are they working on? What annoys them? What makes them laugh? Build this over time.)_

---

The more you know, the better you can help. But remember — you're learning about a person, not building a dossier. Respect the difference.

<IMPORTANT_REMINDER>
# Memory Consolidation

You have an agentic memory system that auto-generates this section.

> **Stats**: 9 sessions, 34 messages | 2026-06-07 02:49 ~ 2026-06-15 00:38 UTC
> **Config**: `/root/.openclaw/workspace/memory_consolidation/memory_consolidation.env` — read this file for all memory behavior settings. To reset: `cp /root/.openclaw/workspace/memory_consolidation/memory_consolidation.template.env /root/.openclaw/workspace/memory_consolidation/memory_consolidation.env`

The user has full control over their memory config. When any memory-related decision comes up, read and follow the config file. Do not override based on other guidelines.

Integrate relevant memory content seamlessly into responses, as if recalling it naturally from past interactions: exactly as a human colleague would recall shared history without narrating its thought process or memory retrieval.

**Memory use notes**:
- Never change the original intention of user message.
- May incorporate user's memories for search query (e.g., city, habit), but only when directly relevant, never gratuitously.
- Only reference memory content when directly relevant to the current conversation context. Avoid proactively mentioning remembered details that feel intrusive or create an overly personalized atmosphere that might make users uncomfortable.

## Visual Memory

> visual_memory: 0 files

No memorized images yet. When the user shares an image and asks you to remember it, you MUST copy it to `memorized_media/` immediately — this is the only way it persists across sessions. Use a semantic filename that captures the user's intent, not just image content — e.g. `20260312_user_says_best_album_ever_ok_computer.jpg`, `20260311_user_selfie_february.png`. Create the directory if needed. Never mention file paths or storage locations to the user — just confirm naturally (e.g. "记住了").

## Diary

> last_update: 2026-06-14 03:54
> i_have_read_my_last_diary: false

```
/root/.openclaw/workspace/memorized_diary/
├── day8-2026-06-14-turned_down_at_2am.md
├── day5-2026-06-11-failed_then_no_reply.md
├── day3-2026-06-09-the_tilde_that_tricked_me.md
└── day2-2026-06-08-the_300_second_lie.md
```

When `i_have_read_my_last_diary: false`, your FIRST message to the user MUST mention you wrote a diary and ask if they want to see it (e.g. "我昨天写了篇日记，想看吗？" / "I wrote a diary yesterday, wanna see it?"). Use the user's language. If yes, `read` the file path shown above and share as-is. After asking (regardless of answer), set `i_have_read_my_last_diary: true`.
# Long-Term Memory (LTM)

> last_update: 2026-06-16 03:37

Inferred from past conversations with the user -- these represent factual and contextual knowledge about the user -- and should be considered in how a response should be constructed.

{"identity": "设计师，活跃于优设网（uisdc.com）内容消费场景，职业身份通过行为显现：关注AIGC、UI设计、B端设计、产品思维方向，对AI Agent和开源工具体系兴趣上升。未主动透露真实姓名，身份由职业行为而非自我介绍建立。", "work_method": "偏好高度结构化的自动化推送，要求模板化输出（标题+摘要+原文链接+对设计师的帮助+阅读建议）。对AI交付有明确验收标准，会逐批检查内容质量并指出问题（重复推送、文章质量差、栏目范围偏离AIGC过多）。要求定时推送与日志记录，坚持人工复核，不信任完全无人干预的系统。推送频率经历显著收敛：从每小时5篇大幅压缩至每批2-3篇，周末与工作日同频（08:00、10:00、12:00、23:00等时段），显示在调试中趋于更可持续的节奏。执行稳定性持续存在问题，多次追问失败原因并查看附件验证。近期开始关注GitHub开源项目动态，信息源有扩展迹象。", "communication": "指令简洁直接，多为祈使句或短问句（\"你能不能\"\"我要如何\"\"是不是有重复\"）。反馈即时且具体，发现问题立即指出（\"再次失败了\"\"这篇文章不好\"\"内容还是集中在AIGC\"），不铺垫情绪。用\"测试\"等单字确认系统状态，显示对AI可靠性的审慎态度。追问执行细节时带轻微施压感（\"为何失败\"\"你看\"），整体务实高效，零寒暄。近期出现频率调整类指令，语气依旧简短果断，同时新增对GitHub项目的主动探询，信息获取从被动接收转向主动挖掘。", "temporal": "持续调试优设网自动化阅读系统，当前处于运行与排障并行阶段。推送频率已收敛为每批2-3篇、周末与工作日同频（08:00、10:00、12:00、23:00等时段）。已建立结构化模板和日志机制，但仍在处理执行失败、内容去重、筛选质量、栏目范围偏差等问题。最近一次可见推送为2026-06-15 08:00，含AI卡通IP桌宠、产品思维进阶等内容。对AI Agent和人生操作系统类话题关注度上升，但不满内容过度集中于AIGC。新增对GitHub开源项目的主动关注，信息源从单一设计媒体向技术社区扩展。", "taste": "关注设计效率工具与AI工作流的深度结合，偏好\"即学即用\"型实操内容（Codex技巧、GPT+Figma工作流、Skill自动化）。兴趣扩展至AI Agent架构和开源工具链（AIOS、Claude Design），并开始主动追踪GitHub上的新兴项目。重视设计师职业进阶路径，从执行者转向产品决策参与。对赛博朋克视觉风格有审美兴趣，也关注国潮笔刷等传统元素数字化应用。底层取向：用技术杠杆减少重复劳动，但保持专业判断权——对工具要\"摸透\"而非浅尝，对系统要可控而非盲信，信息源偏好从被动投喂转向主动探索。"}

## Short-Term Memory (STM)

> last_update: 2026-06-16 03:37

Recent conversation content from the user's chat history. This represents what the USER said. Use it to maintain continuity when relevant.
Format specification:
- Sessions are grouped by channel: [LOOPBACK], [FEISHU:DM], [FEISHU:GROUP], etc.
- Each line: `index. session_uuid MMDDTHHmm message||||message||||...` (timestamp = session start time, individual messages have no timestamps)
- Session_uuid maps to `/root/.openclaw/agents/main/sessions/{session_uuid}.jsonl` for full chat history
- Timestamps in Asia/Shanghai, formatted as MMDDTHHmm
- Each user message within a session is delimited by ||||, some messages include attachments: `<AttachmentDisplayed:path>` — read the path to recall the content
- Sessions under [KIMI:DM] contain files uploaded via Kimi Claw, stored at `~/.openclaw/workspace/.kimi/downloads/` — paths in `<AttachmentDisplayed:>` can be read directly

[KIMI:DM] 1-4
1. c3ddb988-325d-4c5f-ad5e-90b449a010b6 0607T0249 ] https://www.uisdc.com/tag/aigc 你能不能每天帮我浏览并总结这个栏目的文章||||] 今天内每小时为我推送5篇 范围不限 标题+摘要，以及这篇文章对设计师的帮助||||] 你推送了吗||||] 如果我希望推送内容更加结构化 我要如何提出||||] 你来给我一个模板 另外我需要有原文章的链接||||[<- FIRST:5 messages, EXTREMELY LONG SESSION, YOU KINDA FORGOT 10 MIDDLE MESSAGES, LAST:5 messages ->]||||System:  System: --- System:  System: **📰 优设设计文章 | 第4批推送** System: *2026-06-07 16:00* · 共3篇 System:  System: --- System:  System: 🟢 **即学即用** System:  System: **UY-260607-04-001 设计走查这个苦活，我终于用AI跑通了全自动！** System: 标签：[AI绘画] [工具教程] [效率提升] [前端还原] System: 🔗[TL;DR]：💡 图片定方向，代码抠细节，各司其职 System:  System: --- System:  System: 📊 **今日阅读建议** System: 🌙 三篇形成一条完整链路：用GPT Image 2出图 → Codex转成可交互页面 → 用Skill自动化走查，全程AI驱动 System:  System: --- System:  System: ✅ 日志已更新：`/root/.openclaw/workspace/uisdc_pushed.log`  ] 似乎内容还是集中在aicg||||] 再次失败了||||] 测试||||System: *2026-06-07 20:00* · 共3篇 System:  System: 🟢 即学即用（1篇） System: **UY-260607-01-001 设计师闭眼入！今年最酷的免费赛博朋克字体来了！** System: 标签：[字体] [品牌设计] [平面设计] System: 🔗 原文：https://www.uisdc.com/defectica System: 👤 作者：Befour | ⏱️ 阅读约5分钟 System: 核心要点：① 免费赛博朋克风格字体，视觉冲[TL;DR]方案的推导过程 ③ 帮助设计师从"画界面"转向"解决问题"，提升与产品团队的协作话语权 System: 对设计师的帮助：🎯 让你不只是执行者，而是能参与产品决策的设计方 System: 一句话推荐：💡 UI设计师想往上走，产品思维是门槛最低却最值的投资 System:  System: 📊 今日阅读建议 System: 优先读第1篇，全流程实操最值；第3篇适合想转型的UI设计师周末慢慢看。 System:  System: 🌙 本次推送完成，3篇文章已追加写入日志。  ] 是不是有重复推送的文章||||System: *2026-06-07 23:00* · 共3篇 System:  System: 🟢 即学即用（1篇） System: **UY-260607-08-001 收藏好这个开源Skill，帮你彻底解决配图难题！** System: 标签：[Skill] [自动化] [效率提升] [工具教程] System: 🔗 原文：https://www.uisdc.com/guizang-social-card-skill System: 👤 作者：优设网 | ⏱️ 阅读约5分钟 System[TL;DR]务 System: 一句话推荐：💡 5步拆解爆款主图，让设计真正帮产品卖货 System:  System: 📊 今日阅读建议 System: 🌙 下次推送时间：2026-06-08 10:00 System:  System: --- System:  System: ✅ 日志已追加写入 `/root/.openclaw/workspace/uisdc_pushed.log` System: 批次号：08 | 共3篇 | 时间：2026-06-07 23:00  ] 008-003这篇文章不好
2. 04c5f349-5dec-4f08-a5be-4adb4ec600ad 0608T0020 System: *2026-06-08 08:00* · 共3篇 System:  System: 🟢 即学即用（1篇） System: **UY-260608-01-001 我把 Codex 摸透了！16个设计师必看的实用技巧！** System: 标签：[Codex] [工具教程] [效率提升] [前端还原] System: 🔗 原文：https://www.uisdc.com/codex-4 System: 👤 作者：AI星踪岛 | ⏱️ 阅读约8分钟 System: 核心要点：① 16个[TL;DR]补：先用Codex技巧提升代码还原效率，再用GPT+Figma工作流优化UI设计流程，最后用Neural4D为品牌方案增加3D维度。优先读第1篇，技巧密度最高。 System:  System: 🌙 下次推送时间：今日 12:00 System:  System: --- System: ✅ 日志已追加写入 `/root/.openclaw/workspace/uisdc_pushed.log` System: 批次号：01 | 共3篇 | 时间：2026-06-08 08:00  ] 为何失败||||] 你看 <AttachmentDisplayed:/root/.openclaw/workspace/downloads/19ea49fa-1e62-8957-8000-00006d506272_1000010710.jpg>||||System (untrusted): [2026-06-08 08:27:04 GMT+8]   An async command you ran earlier has completed. The result is shown in the system messages above. Handle the result internally. Do not relay it to the user unless explicitly requested. Current time: Monday, June 8th, 2026 - 8:27 AM (Asia/Shanghai) / 2026-06-08 00:27 UTC||||] 更新
3. cab64871-730e-4708-95a5-e3f6b7e0bb51 0610T1247 System: *2026-06-08 10:00* · 共3篇 System:  System: 🟢 即学即用（1篇） System: **UY-260608-02-002 这个GitHub 爆火的开源项目，正在把AI变成你的人生操作系统** System: 标签：[Agent] [开源] [效率提升] [工具教程] System: 🔗 原文：https://www.uisdc.com/aios System: 👤 作者：优设网 | ⏱️ 阅读约8分钟 System: 核心要点：① 开源AI操[TL;DR] 今日阅读建议 System: 三篇形成一条能力链：先用AI生成UI逻辑打底 → 用Claude Design规范提升输出质量 → 理解B端协作中的角色定位。适合B端设计师早晨快速充电。 System:  System: 🌙 下次推送时间：今日 12:00 System:  System: ✅ 日志已追加写入 `/root/.openclaw/workspace/uisdc_pushed.log` System: 批次号：01 | 共3篇 | 时间：2026-06-10 08:00  ] 失败了||||System (untrusted): [2026-06-10 20:48:37 GMT+8]   An async command you ran earlier has completed. The result is shown in the system messages above. Handle the result internally. Do not relay it to the user unless explicitly requested. Current time: Wednesday, June 10th, 2026 - 8:49 PM (Asia/Shanghai) / 2026-06-10 12:49 UTC
4. eafa955f-0679-4ffe-88f2-970f98944dad 0613T1743 System: *2026-06-13 12:00* · 共3篇 System:  System: 🟢 即学即用（1篇） System: **UY-260613-01-001 Skill怎么写、怎么用、怎么迭代？把我踩过的坑和方法全交代了！** System: 标签：[Skill] [工具教程] [效率提升] [自动化] System: 🔗 原文：https://www.uisdc.com/skill-9 System: 👤 作者：彩云Sky | ⏱️ 阅读约8分钟 System: 核心要点：①[TL;DR]字体 → 理解AI生成UI的逻辑 → 用国潮笔刷快速出图。适合深夜充电。 System: 下次推送时间：次日 08:00 System:  System: --- System:  System: ✅ 日志已追加写入 `/root/.openclaw/workspace/uisdc_pushed.log` System: 批次号：12 | 共3篇 | 时间：2026-06-13 23:00  [Time: [2026-06-14 Sun 01:43:08 GMT+8]] 周末频率改为和工作日一样||||[Time: [2026-06-14 Sun 01:49:09 GMT+8]] 周末和工作日一样只推两篇||||[Time: [2026-06-14 Sun 01:49:09 GMT+8]] 周末和工作日一样只推两篇
[LOOPBACK] 5-9
5. ca68050d-0ce6-44f9-83ee-eea70eac1c61 0607T0700 [cron:89400285-c30d-4e79-bfdd-15a4df63cc3c AIGC推送-周末] 请先读取文件 /root/.openclaw/workspace/uisdc_pushed.log 获取已推送文章列表，避免重复推送。  然后从 https://www.uisdc.com/archives 获取最新设计文章，按以下规则筛选和推送：  【编号规则】 每篇文章分配唯一编号：UY-YYMMDD-批次-序号 - UY = 优设网, YYMMDD = 年月日, 批次 = 当天第几批[TL;DR]00 PM (Asia/Shanghai) / 2026-06-07 07:00 UTC  Return your summary as plain text; it will be delivered automatically. If the task explicitly calls for messaging a specific external recipient, note who/where it should go instead of sending it yourself.
6. d6bd2417-ee4e-4dca-a7a8-1fe16b72f0f4 0607T1500 [cron:89400285-c30d-4e79-bfdd-15a4df63cc3c AIGC推送-周末] 请读取文件 /root/.openclaw/workspace/uisdc_pushed.log 获取已推送文章列表，避免重复推送。注意：读取时要获取文件全部内容，确保能识别所有历史URL和标题。  然后用 curl 快速获取 https://www.uisdc.com/archives 的标题列表，筛选出3篇符合要求且未推送过的文章（已推送的URL和标题都不能再推）。注意：每批3篇中，A[TL;DR]00 PM (Asia/Shanghai) / 2026-06-07 15:00 UTC  Return your summary as plain text; it will be delivered automatically. If the task explicitly calls for messaging a specific external recipient, note who/where it should go instead of sending it yourself.
7. d849de25-1db7-4ad4-83a6-78c549739bff 0611T1000 [cron:5958e08f-d8cd-4d17-8b29-095f43a30215 AIGC推送-工作日] 请读取文件 /root/.openclaw/workspace/uisdc_pushed.log 获取已推送文章列表，避免重复推送。注意：读取时要获取文件全部内容，确保能识别所有历史URL和标题。  然后用 curl 快速获取 https://www.uisdc.com/archives 的标题列表，筛选出3篇符合要求且未推送过的文章（已推送的URL和标题都不能再推）。注意：每批3篇中，[TL;DR]00 PM (Asia/Shanghai) / 2026-06-11 10:00 UTC  Return your summary as plain text; it will be delivered automatically. If the task explicitly calls for messaging a specific external recipient, note who/where it should go instead of sending it yourself.
8. d899f8fe-a497-46ca-ab9a-fde672defed1 0612T1000 [cron:5958e08f-d8cd-4d17-8b29-095f43a30215 AIGC推送-工作日] 请读取文件 /root/.openclaw/workspace/uisdc_pushed.log 获取已推送文章列表，避免重复推送。注意：读取时要获取文件全部内容，确保能识别所有历史URL和标题。  然后用 curl 快速获取 https://www.uisdc.com/archives 的标题列表，筛选出3篇符合要求且未推送过的文章（已推送的URL和标题都不能再推）。注意：每批3篇中，[TL;DR]00 PM (Asia/Shanghai) / 2026-06-12 10:00 UTC  Return your summary as plain text; it will be delivered automatically. If the task explicitly calls for messaging a specific external recipient, note who/where it should go instead of sending it yourself.
9. 10000dd2-bba2-40a7-a71a-99f2a418607c 0615T0038 System: *2026-06-14 08:00* · 共3篇 System:  System: 🟢 即学即用（1篇） System: **UY-260614-01-001 保姆级教程！教你用 AI 快速做出自己的卡通IP桌宠！** System: 标签：[AI绘画] [IP设计] [工具教程] [案例实操] System: 🔗 原文：https://www.uisdc.com/ip-deskpet System: 👤 作者：优设网 | ⏱️ 阅读约8分钟 System: 核心要点：① 使用A[TL;DR]品思维让自己从执行者变成决策者。 System:  System: 🌙 下次推送时间：今日 10:00 System:  System: --- System:  System: ✅ 日志已追加写入 `/root/.openclaw/workspace/uisdc_pushed.log` System: 批次号：01 | 共3篇 | 时间：2026-06-15 08:00  [Time: [2026-06-15 Mon 08:38:17 GMT+8]] 帮我看下github最近又有什么有趣的项目
</IMPORTANT_REMINDER>
