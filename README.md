# 172个 GitHub AI / Agent 仓库分类推荐清单

GitHub AI / Agent 仓库分类推荐清单，覆盖图片生成、语音识别、视频自动化、自媒体运营、金融研究、Agent 编程、浏览器自动化、办公工作流等方向。

生成时间：2026-06-08（Asia/Shanghai）

数据来源：用户整理的 GitHub 仓库清单、GitHub REST API、仓库 README/项目描述；非 GitHub 链接仅做入口级判断。GitHub 的 `pushed_at` / 最后提交时间以本次整理记录为准，日期口径可能包含 UTC 与 CST 差异。

排序依据：
1. **工程可用性** — 能否直接用于生产/研究工作流，开箱即用的排前面
2. **生态成熟度** — 插件、文档、社区活跃度、周边工具链是否完善
3. **活跃度** — 最后更新时间，维护频率
4. **许可证清晰度** — MIT/Apache 等清晰许可优先，NOASSERTION/未声明的靠后
5. **落地成本和风险** — 部署复杂度、合规风险、外部依赖多少

排序逻辑：**可直接落地的工具 > 需要二次开发的框架 > 素材集/提示词集/方法论资源**

"免费/开源"只指仓库代码本身；模型 API、云服务、交易所、数据源、GPU/Apple Silicon、本地存储、平台账号等可能另行收费。

<img src="./dh.png" />

## 快速结论

| 目标 | 优先看 | 原因 |
|---|---|---|
| 本地图片 / 封面 / 视觉资产 | ComfyUI、Ideogram4、Infographic | 适合做封面、卡图、信息图和风格一致性素材 |
| 语音识别 / 配音 / 字幕 | Whisper、VoxCPM、VibeVoice、voice-pro | 覆盖转写、TTS、配音、翻译和声音设计 |
| 短视频生成 / 自动剪辑 | MoneyPrinterTurbo、HyperFrames、OpenCut、NarratoAI、Pixelle-Video | 从一键短视频到工程化渲染和后期剪辑都有覆盖 |
| 自媒体采集与分发 | Firecrawl、Scrapling、Agent-Reach、social-auto-upload | 覆盖采集、清洗、跨平台研究和发布 |
| 金融研究 / 交易 Agent | TradingAgents、daily_stock_analysis、FinceptTerminal、Vibe-Trading | 适合投研和回测，实盘需独立风控 |
| 设计 UI / 可视化 | awesome-design-md、open-design、ui-ux-pro-max-skill | 适合沉淀设计规范、原型和可视化资产 |
| 编程 Agent / 工程协作 | OpenClaw、deer-flow、superpowers、ECC、Claude Code | 覆盖长任务、技能、记忆、多 Agent 和工程协作 |
| 浏览器 / 桌面自动化 | agent-s、TuriX-CUA、CloakBrowser、Peekaboo、browser-harness | 扩展 Agent 对真实软件环境的操作能力 |
| 办公 / 低代码工作流 | n8n、Google Workspace CLI、WeChat CLI、Feishu Bridge | 适合连接企业工具、聊天数据和自动化流程 |
| Skills / Prompt / 方法论 | anthropics/skills、agent-skills、Prompt-Engineering-Guide、SkillLens | 适合改造成自己的本地 Skill 库 |

## 📑 目录

- [一、视觉图片与图像提示词（11 个）](#一视觉图片与图像提示词)
- [二、语音音频与配音（6 个）](#二语音音频与配音)
- [三、视频生产、剪辑与数字人（31 个）](#三视频生产剪辑与数字人)
- [四、自媒体内容、采集与分发（16 个）](#四自媒体内容采集与分发)
- [五、金融投研、交易与风控（14 个）](#五金融投研交易与风控)
- [六、设计 UI 与可视化（8 个）](#六设计-ui-与可视化)
- [七、编程 Agent、Skills 与工程协作（35 个）](#七编程-agentskills-与工程协作)
- [八、浏览器/桌面自动化与 Computer Use（9 个）](#八浏览器桌面自动化与-computer-use)
- [九、办公知识工作流与低代码自动化（10 个）](#九办公知识工作流与低代码自动化)
- [十、AI Skills、Prompt 与方法论资产（24 个）](#十ai-skillsprompt-与方法论资产)
- [十一、其他工具、数据源与垂直实验（2 个）](#十一其他工具数据源与垂直实验)
- [十二、非仓库或不可访问 GitHub 入口（6 个）](#十二非仓库或不可访问-github-入口)
- [十三、官网 / 产品页 / 非 GitHub 入口（16 个）](#十三官网--产品页--非-github-入口)
- [十四、注意事项](#十四注意事项)
- [联系方式](#联系方式)

## 一、视觉图片与图像提示词

**1.** **[Comfy-Org/ComfyUI](https://github.com/Comfy-Org/ComfyUI)** — 节点式图像与多模态生成工作流引擎
`Stars: 116.1k` `GPL-3.0` `更新: 2026-06-07`

🏢 Comfy-Org（GitHub 组织账号） · 社区关注度高；由组织账号维护；许可证较清晰（GPL-3.0）；近期仍有更新；部署、显存、模型和节点依赖成本较高，复杂工作流需要学习成本

**2.** **[serengil/deepface](https://github.com/serengil/deepface)** — 人脸识别与人脸属性分析库
`Stars: 22.9k` `MIT` `更新: 2026-05-29`

🏢 serengil（GitHub 个人/小团队账号） · 已有明显社区基础；由个人或小团队维护，迭代可能更灵活；许可证较清晰（MIT）；近期仍有更新；涉及肖像/声音合规和授权风险；模型、GPU 或第三方 API 成本需单独评估

**3.** **[facefusion/facefusion](https://github.com/facefusion/facefusion)** — 人脸融合与换脸工作流工具
`Stars: 28.7k` `NOASSERTION` `更新: 2026-06-07`

🏢 facefusion（GitHub 组织账号） · 已有明显社区基础；由组织账号维护；近期仍有更新；适合补齐 AIGC 生产链路的一环；许可证不清，商用前需核实；涉及肖像/声音合规和授权风险；模型、GPU 或第三方 API 成本需单独评估

**4.** **[EvoLinkAI/awesome-gpt-image-2-API-and-Prompts](https://github.com/EvoLinkAI/awesome-gpt-image-2-API-and-Prompts)** — GPT Image 相关 API 与提示词合集
`Stars: 16.3k` `CC0-1.0` `更新: 2026-06-07`

🏢 EvoLinkAI（GitHub 个人/小团队账号） · 已有明显社区基础；由个人或小团队维护，迭代可能更灵活；许可证较清晰（CC0-1.0）；近期仍有更新；模型、GPU 或第三方 API 成本需单独评估；多数是资产/方法论，不是可直接运行的完整产品

**5.** **[JimLiu/baoyu-skills](https://github.com/JimLiu/baoyu-skills)** — 宝玉风格的 AI Skills 与创作提示资产
`Stars: 20.8k` `未声明` `更新: 2026-06-03`

🏢 JimLiu（GitHub 个人/小团队账号） · 已有明显社区基础；由个人或小团队维护，迭代可能更灵活；近期仍有更新；适合补齐 AIGC 生产链路的一环；许可证不清，商用前需核实；模型、GPU 或第三方 API 成本需单独评估

**6.** **[YouMind-OpenLab/awesome-nano-banana-pro-prompts](https://github.com/YouMind-OpenLab/awesome-nano-banana-pro-prompts)** — Nano Banana Pro 图像提示词资源库
`Stars: 12.4k` `NOASSERTION` `更新: 2026-06-08`

🏢 YouMind-OpenLab（GitHub 组织账号） · 已有明显社区基础；由组织账号维护；近期仍有更新；适合补齐 AIGC 生产链路的一环；许可证不清，商用前需核实；模型、GPU 或第三方 API 成本需单独评估；多数是资产/方法论，不是可直接运行的完整产品

**7.** **[freestylefly/awesome-gpt-image-2](https://github.com/freestylefly/awesome-gpt-image-2)** — GPT Image 2 提示词与模板集合
`Stars: 7.1k` `MIT` `更新: 2026-06-06`

🏢 freestylefly（GitHub 个人/小团队账号） · 已有明显社区基础；由个人或小团队维护，迭代可能更灵活；许可证较清晰（MIT）；近期仍有更新；模型、GPU 或第三方 API 成本需单独评估；多数是资产/方法论，不是可直接运行的完整产品

**8.** **[antvis/Infographic](https://github.com/antvis/Infographic)** — AntV 信息图与可视化模板项目
`Stars: 5.2k` `MIT` `更新: 2026-06-01`

🏢 antvis（GitHub 组织账号） · 已有明显社区基础；由组织账号维护；许可证较清晰（MIT）；近期仍有更新；模型、GPU 或第三方 API 成本需单独评估

**9.** **[YouMind-OpenLab/awesome-gpt-image-2](https://github.com/YouMind-OpenLab/awesome-gpt-image-2)** — GPT Image 2 提示词与案例资源
`Stars: 7.2k` `NOASSERTION` `更新: 2026-06-07`

🏢 YouMind-OpenLab（GitHub 组织账号） · 已有明显社区基础；由组织账号维护；近期仍有更新；适合补齐 AIGC 生产链路的一环；许可证不清，商用前需核实；模型、GPU 或第三方 API 成本需单独评估；多数是资产/方法论，不是可直接运行的完整产品

**10.** **[ideogram-oss/ideogram4](https://github.com/ideogram-oss/ideogram4)** — Ideogram 视觉生成相关开源项目
`Stars: 1.6k` `Apache-2.0` `更新: 2026-06-04`

🏢 ideogram-oss（GitHub 组织账号） · 定位相对聚焦；由组织账号维护；许可证较清晰（Apache-2.0）；近期仍有更新；模型、GPU 或第三方 API 成本需单独评估

**11.** **[liyue-aigc/female-portrait-director](https://github.com/liyue-aigc/female-portrait-director)** — 女性人像视觉生成提示/工作流项目
`Stars: 529` `MIT` `更新: 2026-06-01`

🏢 liyue-aigc（GitHub 个人/小团队账号） · 定位相对聚焦；由个人或小团队维护，迭代可能更灵活；许可证较清晰（MIT）；近期仍有更新；模型、GPU 或第三方 API 成本需单独评估

## 二、语音音频与配音

**1.** **[openai/whisper](https://github.com/openai/whisper)** — OpenAI 开源语音识别模型与转录工具
`Stars: 102.1k` `MIT` `更新: 2026-04-15`

🏢 openai（GitHub 组织账号） · 社区关注度高；由组织账号维护；许可证较清晰（MIT）；近期仍有更新；涉及肖像/声音合规和授权风险；模型、GPU 或第三方 API 成本需单独评估

**2.** **[microsoft/VibeVoice](https://github.com/microsoft/VibeVoice)** — 微软开源语音生成/对话音频模型项目
`Stars: 48.7k` `MIT` `更新: 2026-05-06`

🏢 microsoft（GitHub 组织账号） · 已有明显社区基础；由组织账号维护；许可证较清晰（MIT）；近期仍有更新；涉及肖像/声音合规和授权风险；模型、GPU 或第三方 API 成本需单独评估

**3.** **[OpenBMB/VoxCPM](https://github.com/OpenBMB/VoxCPM)** — OpenBMB 的端到端语音生成模型项目
`Stars: 27.5k` `Apache-2.0` `更新: 2026-05-22`

🏢 OpenBMB（GitHub 组织账号） · 已有明显社区基础；由组织账号维护；许可证较清晰（Apache-2.0）；近期仍有更新；涉及肖像/声音合规和授权风险；模型、GPU 或第三方 API 成本需单独评估

**4.** **[abus-aikorea/voice-pro](https://github.com/abus-aikorea/voice-pro)** — 语音识别、翻译、配音一体化工具
`Stars: 10.6k` `GPL-3.0` `更新: 2025-12-05`

🏢 abus-aikorea（GitHub 个人/小团队账号） · 已有明显社区基础；由个人或小团队维护，迭代可能更灵活；许可证较清晰（GPL-3.0）；适合补齐 AIGC 生产链路的一环；涉及肖像/声音合规和授权风险；模型、GPU 或第三方 API 成本需单独评估

**5.** **[coqui-ai/TTS](https://github.com/coqui-ai/TTS)** — 开源文本转语音训练与推理框架
`Stars: 45.5k` `MPL-2.0` `更新: 2024-08-16`

🏢 coqui-ai（GitHub 组织账号） · 已有明显社区基础；由组织账号维护；许可证较清晰（MPL-2.0）；适合补齐 AIGC 生产链路的一环；最近一年缺少更新；涉及肖像/声音合规和授权风险；模型、GPU 或第三方 API 成本需单独评估

**6.** **[Open-Less/openless](https://github.com/Open-Less/openless)** — 围绕语音/开放模型的本地化工具项目
`Stars: 2.2k` `MIT` `更新: 2026-06-08`

🏢 Open-Less（GitHub 组织账号） · 定位相对聚焦；由组织账号维护；许可证较清晰（MIT）；近期仍有更新；涉及肖像/声音合规和授权风险；模型、GPU 或第三方 API 成本需单独评估

## 三、视频生产、剪辑与数字人

**1.** **[hacksider/Deep-Live-Cam](https://github.com/hacksider/Deep-Live-Cam)** — 实时人脸替换与视频换脸工具
`Stars: 93.7k` `AGPL-3.0` `更新: 2026-05-31`

🏢 hacksider（GitHub 个人/小团队账号） · 社区关注度高；由个人或小团队维护，迭代可能更灵活；许可证较清晰（AGPL-3.0）；近期仍有更新；涉及肖像/声音合规和授权风险；模型、GPU 或第三方 API 成本需单独评估

**2.** **[harry0703/MoneyPrinterTurbo](https://github.com/harry0703/MoneyPrinterTurbo)** — 大模型驱动的一键短视频生成工具
`Stars: 81.2k` `MIT` `更新: 2026-06-06`

🏢 harry0703（GitHub 个人/小团队账号） · 社区关注度高；由个人或小团队维护，迭代可能更灵活；许可证较清晰（MIT）；近期仍有更新；模型、GPU 或第三方 API 成本需单独评估

**3.** **[OpenCut-app/OpenCut](https://github.com/OpenCut-app/OpenCut)** — 开源视频编辑器
`Stars: 54.8k` `MIT` `更新: 2026-05-27`

🏢 OpenCut-app（GitHub 组织账号） · 社区关注度高；由组织账号维护；许可证较清晰（MIT）；近期仍有更新；模型、GPU 或第三方 API 成本需单独评估

**4.** **[soimort/you-get](https://github.com/soimort/you-get)** — 命令行视频/媒体下载工具
`Stars: 56.8k` `NOASSERTION` `更新: 2026-04-30`

🏢 soimort（GitHub 个人/小团队账号） · 社区关注度高；由个人或小团队维护，迭代可能更灵活；近期仍有更新；适合补齐 AIGC 生产链路的一环；许可证不清，商用前需核实；模型、GPU 或第三方 API 成本需单独评估

**5.** **[heygen-com/hyperframes](https://github.com/heygen-com/hyperframes)** — 将 HTML/网页内容渲染为视频的工程工具
`Stars: 25.4k` `Apache-2.0` `更新: 2026-06-08`

🏢 heygen-com（GitHub 组织账号） · 已有明显社区基础；由组织账号维护；许可证较清晰（Apache-2.0）；近期仍有更新；模型、GPU 或第三方 API 成本需单独评估

**6.** **[AIDC-AI/Pixelle-Video](https://github.com/AIDC-AI/Pixelle-Video)** — AI 全自动短视频生产引擎
`Stars: 21.7k` `Apache-2.0` `更新: 2026-06-03`

🏢 AIDC-AI（GitHub 组织账号） · 已有明显社区基础；由组织账号维护；许可证较清晰（Apache-2.0）；近期仍有更新；涉及肖像/声音合规和授权风险；模型、GPU 或第三方 API 成本需单独评估

**7.** **[elebumm/RedditVideoMakerBot](https://github.com/elebumm/RedditVideoMakerBot)** — Reddit 内容转短视频机器人
`Stars: 12.4k` `GPL-3.0` `更新: 2026-05-25`

🏢 elebumm（GitHub 个人/小团队账号） · 已有明显社区基础；由个人或小团队维护，迭代可能更灵活；许可证较清晰（GPL-3.0）；近期仍有更新；模型、GPU 或第三方 API 成本需单独评估

**8.** **[HBAI-Ltd/Toonflow-app](https://github.com/HBAI-Ltd/Toonflow-app)** — 小说/剧本到动画短剧的一站式桌面工具
`Stars: 9.7k` `Apache-2.0` `更新: 2026-06-07`

🏢 HBAI-Ltd（GitHub 个人/小团队账号） · 已有明显社区基础；由个人或小团队维护，迭代可能更灵活；许可证较清晰（Apache-2.0）；近期仍有更新；模型、GPU 或第三方 API 成本需单独评估

**9.** **[browser-use/video-use](https://github.com/browser-use/video-use)** — Browser Use 团队的视频自动剪辑 Agent
`Stars: 9.2k` `MIT` `更新: 2026-05-15`

🏢 browser-use（GitHub 组织账号） · 已有明显社区基础；由组织账号维护；许可证较清晰（MIT）；近期仍有更新；模型、GPU 或第三方 API 成本需单独评估

**10.** **[HKUDS/ViMax](https://github.com/HKUDS/ViMax)** — Agent 化视频生成工作流
`Stars: 9.0k` `MIT` `更新: 2026-06-01`

🏢 HKUDS（GitHub 组织账号） · 已有明显社区基础；由组织账号维护；许可证较清晰（MIT）；近期仍有更新；模型、GPU 或第三方 API 成本需单独评估

**11.** **[chatfire-AI/huobao-drama](https://github.com/chatfire-AI/huobao-drama)** — AI 短剧生成平台
`Stars: 12.6k` `未声明` `更新: 2026-05-21`

🏢 chatfire-AI（GitHub 组织账号） · 已有明显社区基础；由组织账号维护；近期仍有更新；适合补齐 AIGC 生产链路的一环；许可证不清，商用前需核实；模型、GPU 或第三方 API 成本需单独评估

**12.** **[lipku/LiveTalking](https://github.com/lipku/LiveTalking)** — 实时数字人口型驱动项目
`Stars: 7.9k` `Apache-2.0` `更新: 2026-06-07`

🏢 lipku（GitHub 个人/小团队账号） · 已有明显社区基础；由个人或小团队维护，迭代可能更灵活；许可证较清晰（Apache-2.0）；近期仍有更新；模型、GPU 或第三方 API 成本需单独评估

**13.** **[MeiGen-AI/InfiniteTalk](https://github.com/MeiGen-AI/InfiniteTalk)** — 长时长/多轮数字人说话视频生成项目
`Stars: 6.8k` `Apache-2.0` `更新: 2026-05-22`

🏢 MeiGen-AI（GitHub 组织账号） · 已有明显社区基础；由组织账号维护；许可证较清晰（Apache-2.0）；近期仍有更新；模型、GPU 或第三方 API 成本需单独评估

**14.** **[linyqh/NarratoAI](https://github.com/linyqh/NarratoAI)** — AI 影视解说与自动剪辑工作流
`Stars: 9.7k` `NOASSERTION` `更新: 2026-06-04`

🏢 linyqh（GitHub 个人/小团队账号） · 已有明显社区基础；由个人或小团队维护，迭代可能更灵活；近期仍有更新；适合补齐 AIGC 生产链路的一环；许可证不清，商用前需核实；模型、GPU 或第三方 API 成本需单独评估

**15.** **[zhouxiaoka/autoclip](https://github.com/zhouxiaoka/autoclip)** — 视频高光切片自动化工具
`Stars: 5.6k` `MIT` `更新: 2026-06-03`

🏢 zhouxiaoka（GitHub 个人/小团队账号） · 已有明显社区基础；由个人或小团队维护，迭代可能更灵活；许可证较清晰（MIT）；近期仍有更新；模型、GPU 或第三方 API 成本需单独评估

**16.** **[meituan-longcat/LongCat-Video](https://github.com/meituan-longcat/LongCat-Video)** — 美团 LongCat 视频生成相关项目
`Stars: 4.2k` `MIT` `更新: 2026-05-27`

🏢 meituan-longcat（GitHub 组织账号） · 定位相对聚焦；由组织账号维护；许可证较清晰（MIT）；近期仍有更新；模型、GPU 或第三方 API 成本需单独评估

**17.** **[ltaoo/wx_channels_download](https://github.com/ltaoo/wx_channels_download)** — 视频号下载工具
`Stars: 6.4k` `NOASSERTION` `更新: 2026-06-07`

🏢 ltaoo（GitHub 个人/小团队账号） · 已有明显社区基础；由个人或小团队维护，迭代可能更灵活；近期仍有更新；适合补齐 AIGC 生产链路的一环；许可证不清，商用前需核实；模型、GPU 或第三方 API 成本需单独评估

**18.** **[Forget-C/Jellyfish](https://github.com/Forget-C/Jellyfish)** — AI 短剧端到端生产工作台
`Stars: 3.8k` `Apache-2.0` `更新: 2026-04-20`

🏢 Forget-C（GitHub 个人/小团队账号） · 定位相对聚焦；由个人或小团队维护，迭代可能更灵活；许可证较清晰（Apache-2.0）；近期仍有更新；模型、GPU 或第三方 API 成本需单独评估

**19.** **[MemeCalculate/moyin-creator](https://github.com/MemeCalculate/moyin-creator)** — AI 影视生产与创作工具
`Stars: 3.7k` `AGPL-3.0` `更新: 2026-05-26`

🏢 MemeCalculate（GitHub 组织账号） · 定位相对聚焦；由组织账号维护；许可证较清晰（AGPL-3.0）；近期仍有更新；模型、GPU 或第三方 API 成本需单独评估

**20.** **[remotion-dev/skills](https://github.com/remotion-dev/skills)** — Remotion 视频生成相关 Skills
`Stars: 3.5k` `未声明` `更新: 2026-05-07`

🏢 remotion-dev（GitHub 组织账号） · 定位相对聚焦；由组织账号维护；近期仍有更新；适合补齐 AIGC 生产链路的一环；许可证不清，商用前需核实；模型、GPU 或第三方 API 成本需单独评估

**21.** **[Kedreamix/Linly-Talker](https://github.com/Kedreamix/Linly-Talker)** — 数字人口型同步与说话人视频工具
`Stars: 3.3k` `MIT` `更新: 2026-02-10`

🏢 Kedreamix（GitHub 个人/小团队账号） · 定位相对聚焦；由个人或小团队维护，迭代可能更灵活；许可证较清晰（MIT）；近期仍有更新；涉及肖像/声音合规和授权风险；模型、GPU 或第三方 API 成本需单独评估

**22.** **[AliaksandrSiarohin/first-order-model](https://github.com/AliaksandrSiarohin/first-order-model)** — 经典一阶运动模型，支持参考图驱动动作迁移
`Stars: 15.0k` `MIT` `更新: 2024-11-14`

🏢 AliaksandrSiarohin（GitHub 个人/小团队账号） · 已有明显社区基础；由个人或小团队维护，迭代可能更灵活；许可证较清晰（MIT）；适合补齐 AIGC 生产链路的一环；最近一年缺少更新；模型、GPU 或第三方 API 成本需单独评估

**23.** **[NarratorAI-Studio/narrator-ai-cli-skill](https://github.com/NarratorAI-Studio/narrator-ai-cli-skill)** — AI 解说与视频旁白生成 Skill
`Stars: 716` `MIT` `更新: 2026-06-03`

🏢 NarratorAI-Studio（GitHub 组织账号） · 定位相对聚焦；由组织账号维护；许可证较清晰（MIT）；近期仍有更新；模型、GPU 或第三方 API 成本需单独评估

**24.** **[dexhunter/seedance2-skill](https://github.com/dexhunter/seedance2-skill)** — Seedance 视频模型调用 Skill
`Stars: 1.4k` `MIT` `更新: 2026-02-18`

🏢 dexhunter（GitHub 个人/小团队账号） · 定位相对聚焦；由个人或小团队维护，迭代可能更灵活；许可证较清晰（MIT）；近期仍有更新；模型、GPU 或第三方 API 成本需单独评估

**25.** **[Geniusay/ChopperBot](https://github.com/Geniusay/ChopperBot)** — 直播高光切片、封面、发布自动化机器人
`Stars: 2.7k` `Apache-2.0` `更新: 2025-08-04`

🏢 Geniusay（GitHub 个人/小团队账号） · 定位相对聚焦；由个人或小团队维护，迭代可能更灵活；许可证较清晰（Apache-2.0）；适合补齐 AIGC 生产链路的一环；模型、GPU 或第三方 API 成本需单独评估

**26.** **[PeterL1n/BackgroundMattingV2](https://github.com/PeterL1n/BackgroundMattingV2)** — 高质量人像抠图与背景替换模型
`Stars: 7.2k` `MIT` `更新: 2024-06-19`

🏢 PeterL1n（GitHub 个人/小团队账号） · 已有明显社区基础；由个人或小团队维护，迭代可能更灵活；许可证较清晰（MIT）；适合补齐 AIGC 生产链路的一环；最近一年缺少更新；模型、GPU 或第三方 API 成本需单独评估

**27.** **[MeiGen-AI/LongCat-Video-Avatar](https://github.com/MeiGen-AI/LongCat-Video-Avatar)** — LongCat 视频数字人项目
`Stars: 300` `未声明` `更新: 2025-12-18`

🏢 MeiGen-AI（GitHub 组织账号） · 定位相对聚焦；由组织账号维护；近期仍有更新；适合补齐 AIGC 生产链路的一环；许可证不清，商用前需核实；社区验证样本偏少；涉及肖像/声音合规和授权风险；模型、GPU 或第三方 API 成本需单独评估

**28.** **[happyhorseai/happyhorse](https://github.com/happyhorseai/happyhorse)** — 面向视频/创意生产的 AI 工具项目
`Stars: 136` `未声明` `更新: 2026-04-08`

🏢 happyhorseai（GitHub 组织账号） · 定位相对聚焦；由组织账号维护；近期仍有更新；适合补齐 AIGC 生产链路的一环；许可证不清，商用前需核实；社区验证样本偏少；模型、GPU 或第三方 API 成本需单独评估

**29.** **[jianshuo/claude-skills](https://github.com/jianshuo/claude-skills)** — 视频创作相关 Claude Skills
`Stars: 77` `MIT` `更新: 2026-06-07`

🏢 jianshuo（GitHub 个人/小团队账号） · 定位相对聚焦；由个人或小团队维护，迭代可能更灵活；许可证较清晰（MIT）；近期仍有更新；社区验证样本偏少；模型、GPU 或第三方 API 成本需单独评估

**30.** **[alecm20/story-flicks](https://github.com/alecm20/story-flicks)** — 输入故事主题生成故事视频的项目
`Stars: 2.4k` `未声明` `更新: 2025-03-12`

🏢 alecm20（GitHub 个人/小团队账号） · 定位相对聚焦；由个人或小团队维护，迭代可能更灵活；适合补齐 AIGC 生产链路的一环；许可证不清，商用前需核实；最近一年缺少更新；模型、GPU 或第三方 API 成本需单独评估

**31.** **[yuanzhongqiao/deep-comedy-pro](https://github.com/yuanzhongqiao/deep-comedy-pro)** — AI 漫剧/短剧生产工具
`Stars: 7` `未声明` `更新: 2026-06-04`

🏢 yuanzhongqiao（GitHub 个人/小团队账号） · 定位相对聚焦；由个人或小团队维护，迭代可能更灵活；近期仍有更新；适合补齐 AIGC 生产链路的一环；许可证不清，商用前需核实；社区验证样本偏少；模型、GPU 或第三方 API 成本需单独评估

## 四、自媒体内容、采集与分发

**1.** **[firecrawl/firecrawl](https://github.com/firecrawl/firecrawl)** — 网页搜索、抓取与结构化提取 API/平台
`Stars: 129.9k` `AGPL-3.0` `更新: 2026-06-07`

🏢 firecrawl（GitHub 组织账号） · 社区关注度高；由组织账号维护；许可证较清晰（AGPL-3.0）；近期仍有更新；仍需阅读 README、Issue 和依赖清单后再决定集成

**2.** **[D4Vinci/Scrapling](https://github.com/D4Vinci/Scrapling)** — 自适应 Web Scraping 框架
`Stars: 61.9k` `BSD-3-Clause` `更新: 2026-06-07`

🏢 D4Vinci（GitHub 个人/小团队账号） · 社区关注度高；由个人或小团队维护，迭代可能更灵活；许可证较清晰（BSD-3-Clause）；近期仍有更新；仍需阅读 README、Issue 和依赖清单后再决定集成

**3.** **[NaiboWang/EasySpider](https://github.com/NaiboWang/EasySpider)** — 可视化爬虫/网页采集工具
`Stars: 43.9k` `AGPL-3.0` `更新: 2026-05-22`

🏢 NaiboWang（GitHub 个人/小团队账号） · 已有明显社区基础；由个人或小团队维护，迭代可能更灵活；许可证较清晰（AGPL-3.0）；近期仍有更新；仍需阅读 README、Issue 和依赖清单后再决定集成

**4.** **[mvanhorn/last30days-skill](https://github.com/mvanhorn/last30days-skill)** — 近期热点追踪 Skill
`Stars: 31.2k` `MIT` `更新: 2026-06-06`

🏢 mvanhorn（GitHub 个人/小团队账号） · 已有明显社区基础；由个人或小团队维护，迭代可能更灵活；许可证较清晰（MIT）；近期仍有更新；仍需阅读 README、Issue 和依赖清单后再决定集成

**5.** **[Panniantong/Agent-Reach](https://github.com/Panniantong/Agent-Reach)** — 为 Agent 接入搜索、社媒、GitHub 等互联网能力
`Stars: 23.2k` `MIT` `更新: 2026-05-18`

🏢 Panniantong（GitHub 个人/小团队账号） · 已有明显社区基础；由个人或小团队维护，迭代可能更灵活；许可证较清晰（MIT）；近期仍有更新；仍需阅读 README、Issue 和依赖清单后再决定集成

**6.** **[yikart/AiToEarn](https://github.com/yikart/AiToEarn)** — 一人公司内容营销 Agent
`Stars: 18.8k` `MIT` `更新: 2026-05-21`

🏢 yikart（GitHub 组织账号） · 已有明显社区基础；由组织账号维护；许可证较清晰（MIT）；近期仍有更新；仍需阅读 README、Issue 和依赖清单后再决定集成

**7.** **[KKKKhazix/khazix-skills](https://github.com/KKKKhazix/khazix-skills)** — 面向内容创作的 Skills 集合
`Stars: 14.0k` `MIT` `更新: 2026-06-04`

🏢 KKKKhazix（GitHub 个人/小团队账号） · 已有明显社区基础；由个人或小团队维护，迭代可能更灵活；许可证较清晰（MIT）；近期仍有更新；仍需阅读 README、Issue 和依赖清单后再决定集成

**8.** **[dreammis/social-auto-upload](https://github.com/dreammis/social-auto-upload)** — 多平台社媒自动发布工具
`Stars: 12.4k` `未声明` `更新: 2026-06-05`

🏢 dreammis（GitHub 个人/小团队账号） · 已有明显社区基础；由个人或小团队维护，迭代可能更灵活；近期仍有更新；贴近内容团队的采集到发布流程；许可证不清，商用前需核实

**9.** **[joeseesun/qiaomu-anything-to-notebooklm](https://github.com/joeseesun/qiaomu-anything-to-notebooklm)** — 把多源内容转成播客、PPT、思维导图和测验
`Stars: 5.0k` `MIT` `更新: 2026-04-28`

🏢 joeseesun（GitHub 个人/小团队账号） · 定位相对聚焦；由个人或小团队维护，迭代可能更灵活；许可证较清晰（MIT）；近期仍有更新；仍需阅读 README、Issue 和依赖清单后再决定集成

**10.** **[op7418/Humanizer-zh](https://github.com/op7418/Humanizer-zh)** — 中文文本去 AI 味改写工具
`Stars: 9.5k` `MIT` `更新: 2026-01-19`

🏢 op7418（GitHub 个人/小团队账号） · 已有明显社区基础；由个人或小团队维护，迭代可能更灵活；许可证较清晰（MIT）；近期仍有更新；仍需阅读 README、Issue 和依赖清单后再决定集成

**11.** **[geekjourneyx/md2wechat-skill](https://github.com/geekjourneyx/md2wechat-skill)** — Markdown 转微信公众号排版 Skill
`Stars: 2.8k` `NOASSERTION` `更新: 2026-06-07`

🏢 geekjourneyx（GitHub 个人/小团队账号） · 定位相对聚焦；由个人或小团队维护，迭代可能更灵活；近期仍有更新；贴近内容团队的采集到发布流程；许可证不清，商用前需核实

**12.** **[jackwener/xiaohongshu-cli](https://github.com/jackwener/xiaohongshu-cli)** — 小红书命令行工具
`Stars: 2.1k` `未声明` `更新: 2026-03-21`

🏢 jackwener（GitHub 个人/小团队账号） · 定位相对聚焦；由个人或小团队维护，迭代可能更灵活；近期仍有更新；贴近内容团队的采集到发布流程；许可证不清，商用前需核实

**13.** **[huangserva/skill-prompt-generator](https://github.com/huangserva/skill-prompt-generator)** — 基于 Skills 的提示词生成系统
`Stars: 1.4k` `未声明` `更新: 2026-05-10`

🏢 huangserva（GitHub 个人/小团队账号） · 定位相对聚焦；由个人或小团队维护，迭代可能更灵活；近期仍有更新；贴近内容团队的采集到发布流程；许可证不清，商用前需核实

**14.** **[CheeMao/ai-content](https://github.com/CheeMao/ai-content)** — AI 内容生产、选题、卡图和发布系统
`Stars: 263` `NOASSERTION` `更新: 2026-03-20`

🏢 CheeMao（GitHub 个人/小团队账号） · 定位相对聚焦；由个人或小团队维护，迭代可能更灵活；近期仍有更新；贴近内容团队的采集到发布流程；许可证不清，商用前需核实；社区验证样本偏少

**15.** **[zjp1997720/wechat-radar](https://github.com/zjp1997720/wechat-radar)** — 微信内容监测/雷达工具
`Stars: 94` `MIT` `更新: 2026-05-26`

🏢 zjp1997720（GitHub 个人/小团队账号） · 定位相对聚焦；由个人或小团队维护，迭代可能更灵活；许可证较清晰（MIT）；近期仍有更新；社区验证样本偏少

**16.** **[hekaixin66-sketch/xiaohongshuritter](https://github.com/hekaixin66-sketch/xiaohongshuritter)** — 企业级小红书 MCP/多账号运营系统
`Stars: 132` `未声明` `更新: 2026-04-05`

🏢 hekaixin66-sketch（GitHub 个人/小团队账号） · 定位相对聚焦；由个人或小团队维护，迭代可能更灵活；近期仍有更新；贴近内容团队的采集到发布流程；许可证不清，商用前需核实；社区验证样本偏少

## 五、金融投研、交易与风控

**1.** **[TauricResearch/TradingAgents](https://github.com/TauricResearch/TradingAgents)** — 多智能体 LLM 金融交易框架
`Stars: 84.1k` `Apache-2.0` `更新: 2026-06-01`

🏢 TauricResearch（GitHub 组织账号） · 社区关注度高；由组织账号维护；许可证较清晰（Apache-2.0）；近期仍有更新；不能直接等同于可实盘盈利系统，数据源和风控需重建

**2.** **[ZhuLinsen/daily_stock_analysis](https://github.com/ZhuLinsen/daily_stock_analysis)** — 每日股票智能分析系统
`Stars: 41.2k` `MIT` `更新: 2026-06-07`

🏢 ZhuLinsen（GitHub 个人/小团队账号） · 已有明显社区基础；由个人或小团队维护，迭代可能更灵活；许可证较清晰（MIT）；近期仍有更新；不能直接等同于可实盘盈利系统，数据源和风控需重建

**3.** **[koala73/worldmonitor](https://github.com/koala73/worldmonitor)** — 全球情报与事件监控仪表板
`Stars: 56.0k` `NOASSERTION` `更新: 2026-06-07`

🏢 koala73（GitHub 个人/小团队账号） · 社区关注度高；由个人或小团队维护，迭代可能更灵活；近期仍有更新；适合先做研究/回测/投研辅助验证；许可证不清，商用前需核实；涉及肖像/声音合规和授权风险；不能直接等同于可实盘盈利系统，数据源和风控需重建

**4.** **[anthropics/financial-services](https://github.com/anthropics/financial-services)** — Anthropic 面向金融服务场景的 Skills/参考资产
`Stars: 30.4k` `Apache-2.0` `更新: 2026-06-05`

🏢 anthropics（GitHub 组织账号） · 已有明显社区基础；由组织账号维护；许可证较清晰（Apache-2.0）；近期仍有更新；不能直接等同于可实盘盈利系统，数据源和风控需重建

**5.** **[shiyu-coder/Kronos](https://github.com/shiyu-coder/Kronos)** — 金融时间序列/交易相关模型项目
`Stars: 28.9k` `MIT` `更新: 2026-04-13`

🏢 shiyu-coder（GitHub 个人/小团队账号） · 已有明显社区基础；由个人或小团队维护，迭代可能更灵活；许可证较清晰（MIT）；近期仍有更新；不能直接等同于可实盘盈利系统，数据源和风控需重建

**6.** **[virattt/dexter](https://github.com/virattt/dexter)** — 把金融问题拆成研究计划的 Agent
`Stars: 26.9k` `未声明` `更新: 2026-06-03`

🏢 virattt（GitHub 个人/小团队账号） · 已有明显社区基础；由个人或小团队维护，迭代可能更灵活；近期仍有更新；适合先做研究/回测/投研辅助验证；许可证不清，商用前需核实；不能直接等同于可实盘盈利系统，数据源和风控需重建

**7.** **[Fincept-Corporation/FinceptTerminal](https://github.com/Fincept-Corporation/FinceptTerminal)** — 金融终端、市场分析和经济数据探索应用
`Stars: 25.9k` `NOASSERTION` `更新: 2026-06-05`

🏢 Fincept-Corporation（GitHub 组织账号） · 已有明显社区基础；由组织账号维护；近期仍有更新；适合先做研究/回测/投研辅助验证；许可证不清，商用前需核实；不能直接等同于可实盘盈利系统，数据源和风控需重建

**8.** **[Open-Dev-Society/OpenStock](https://github.com/Open-Dev-Society/OpenStock)** — 开源股票盯盘与行情分析工具
`Stars: 13.1k` `AGPL-3.0` `更新: 2026-05-28`

🏢 Open-Dev-Society（GitHub 组织账号） · 已有明显社区基础；由组织账号维护；许可证较清晰（AGPL-3.0）；近期仍有更新；不能直接等同于可实盘盈利系统，数据源和风控需重建

**9.** **[HKUDS/Vibe-Trading](https://github.com/HKUDS/Vibe-Trading)** — 个人交易智能体项目
`Stars: 11.1k` `MIT` `更新: 2026-06-06`

🏢 HKUDS（GitHub 组织账号） · 已有明显社区基础；由组织账号维护；许可证较清晰（MIT）；近期仍有更新；不能直接等同于可实盘盈利系统，数据源和风控需重建

**10.** **[leanprover/lean4](https://github.com/leanprover/lean4)** — 形式化证明语言和定理证明器，可用于严谨验证
`Stars: 8.2k` `Apache-2.0` `更新: 2026-06-07`

🏢 leanprover（GitHub 组织账号） · 已有明显社区基础；由组织账号维护；许可证较清晰（Apache-2.0）；近期仍有更新；不能直接等同于可实盘盈利系统，数据源和风控需重建

**11.** **[brokermr810/QuantDinger](https://github.com/brokermr810/QuantDinger)** — 量化交易系统
`Stars: 7.5k` `Apache-2.0` `更新: 2026-06-06`

🏢 brokermr810（GitHub 个人/小团队账号） · 已有明显社区基础；由个人或小团队维护，迭代可能更灵活；许可证较清晰（Apache-2.0）；近期仍有更新；不能直接等同于可实盘盈利系统，数据源和风控需重建

**12.** **[bwjoke/BTC-Trading-Since-2020](https://github.com/bwjoke/BTC-Trading-Since-2020)** — BTC 交易记录/策略复盘项目
`Stars: 1.2k` `未声明` `更新: 2026-05-03`

🏢 bwjoke（GitHub 个人/小团队账号） · 定位相对聚焦；由个人或小团队维护，迭代可能更灵活；近期仍有更新；适合先做研究/回测/投研辅助验证；许可证不清，商用前需核实；不能直接等同于可实盘盈利系统，数据源和风控需重建

**13.** **[AlphaGBM/skills](https://github.com/AlphaGBM/skills)** — 面向期权/金融数据的 AI Skills
`Stars: 696` `MIT` `更新: 2026-05-27`

🏢 AlphaGBM（GitHub 个人/小团队账号） · 定位相对聚焦；由个人或小团队维护，迭代可能更灵活；许可证较清晰（MIT）；近期仍有更新；不能直接等同于可实盘盈利系统，数据源和风控需重建

**14.** **[okx/agent-trade-kit](https://github.com/okx/agent-trade-kit)** — OKX 面向 AI Agent 的交易工具集
`Stars: 325` `MIT` `更新: 2026-06-05`

🏢 okx（GitHub 组织账号） · 定位相对聚焦；由组织账号维护；许可证较清晰（MIT）；近期仍有更新；社区验证样本偏少；不能直接等同于可实盘盈利系统，数据源和风控需重建

## 六、设计 UI 与可视化

**1.** **[nextlevelbuilder/ui-ux-pro-max-skill](https://github.com/nextlevelbuilder/ui-ux-pro-max-skill)** — 面向多平台 UI/UX 的设计智能 Skill
`Stars: 88.6k` `MIT` `更新: 2026-04-03`

🏢 nextlevelbuilder（GitHub 组织账号） · 社区关注度高；由组织账号维护；许可证较清晰（MIT）；近期仍有更新；仍需阅读 README、Issue 和依赖清单后再决定集成

**2.** **[VoltAgent/awesome-design-md](https://github.com/VoltAgent/awesome-design-md)** — 收集品牌 DESIGN.md，辅助 Agent 做一致性设计
`Stars: 88.2k` `MIT` `更新: 2026-05-30`

🏢 VoltAgent（GitHub 组织账号） · 社区关注度高；由组织账号维护；许可证较清晰（MIT）；近期仍有更新；多数是资产/方法论，不是可直接运行的完整产品

**3.** **[nexu-io/open-design](https://github.com/nexu-io/open-design)** — 开源设计系统/设计协作项目
`Stars: 61.0k` `Apache-2.0` `更新: 2026-06-08`

🏢 nexu-io（GitHub 组织账号） · 社区关注度高；由组织账号维护；许可证较清晰（Apache-2.0）；近期仍有更新；仍需阅读 README、Issue 和依赖清单后再决定集成

**4.** **[Leonxlnx/taste-skill](https://github.com/Leonxlnx/taste-skill)** — 审美与 UI 质量评估 Skill
`Stars: 36.8k` `MIT` `更新: 2026-05-26`

🏢 Leonxlnx（GitHub 个人/小团队账号） · 已有明显社区基础；由个人或小团队维护，迭代可能更灵活；许可证较清晰（MIT）；近期仍有更新；仍需阅读 README、Issue 和依赖清单后再决定集成

**5.** **[JCodesMore/ai-website-cloner-template](https://github.com/JCodesMore/ai-website-cloner-template)** — AI 网站克隆模板
`Stars: 16.5k` `MIT` `更新: 2026-06-01`

🏢 JCodesMore（GitHub 个人/小团队账号） · 已有明显社区基础；由个人或小团队维护，迭代可能更灵活；许可证较清晰（MIT）；近期仍有更新；仍需阅读 README、Issue 和依赖清单后再决定集成

**6.** **[guokaigdg/animal-island-ui](https://github.com/guokaigdg/animal-island-ui)** — 主题化 UI 组件/示例项目
`Stars: 3.1k` `MIT` `更新: 2026-06-07`

🏢 guokaigdg（GitHub 个人/小团队账号） · 定位相对聚焦；由个人或小团队维护，迭代可能更灵活；许可证较清晰（MIT）；近期仍有更新；仍需阅读 README、Issue 和依赖清单后再决定集成

**7.** **[antvis/chart-visualization-skills](https://github.com/antvis/chart-visualization-skills)** — AntV 图表可视化 Skills
`Stars: 335` `MIT` `更新: 2026-06-04`

🏢 antvis（GitHub 组织账号） · 定位相对聚焦；由组织账号维护；许可证较清晰（MIT）；近期仍有更新；社区验证样本偏少

**8.** **[ant-design/antd-skill](https://github.com/ant-design/antd-skill)** — Ant Design 相关 Agent Skill
`Stars: 95` `MIT` `更新: 2026-03-27`

🏢 ant-design（GitHub 组织账号） · 定位相对聚焦；由组织账号维护；许可证较清晰（MIT）；近期仍有更新；社区验证样本偏少

## 七、编程 Agent、Skills 与工程协作

**1.** **[openclaw/openclaw](https://github.com/openclaw/openclaw)** — 跨平台个人 AI 助手/Agent 平台
`Stars: 377.5k` `NOASSERTION` `更新: 2026-06-08`

🏢 openclaw（GitHub 组织账号） · 社区关注度高；由组织账号维护；近期仍有更新；便于沉淀为可复用 Agent 工作流；许可证不清，商用前需核实

**2.** **[obra/superpowers](https://github.com/obra/superpowers)** — Agentic Skills 方法论与开发流程框架
`Stars: 220.5k` `MIT` `更新: 2026-06-03`

🏢 obra（GitHub 个人/小团队账号） · 社区关注度高；由个人或小团队维护，迭代可能更灵活；许可证较清晰（MIT）；近期仍有更新；仍需阅读 README、Issue 和依赖清单后再决定集成

**3.** **[affaan-m/ECC](https://github.com/affaan-m/ECC)** — Claude Code/Codex 等 Agent 的性能优化与技能体系
`Stars: 209.9k` `MIT` `更新: 2026-06-07`

🏢 affaan-m（GitHub 个人/小团队账号） · 社区关注度高；由个人或小团队维护，迭代可能更灵活；许可证较清晰（MIT）；近期仍有更新；仍需阅读 README、Issue 和依赖清单后再决定集成

**4.** **[NousResearch/hermes-agent](https://github.com/NousResearch/hermes-agent)** — 可成长的个人 Agent
`Stars: 186.0k` `MIT` `更新: 2026-06-08`

🏢 NousResearch（GitHub 组织账号） · 社区关注度高；由组织账号维护；许可证较清晰（MIT）；近期仍有更新；仍需阅读 README、Issue 和依赖清单后再决定集成

**5.** **[msitarzewski/agency-agents](https://github.com/msitarzewski/agency-agents)** — 面向 AI Agency 的专家 Agent 集合
`Stars: 108.1k` `MIT` `更新: 2026-06-07`

🏢 msitarzewski（GitHub 个人/小团队账号） · 社区关注度高；由个人或小团队维护，迭代可能更灵活；许可证较清晰（MIT）；近期仍有更新；仍需阅读 README、Issue 和依赖清单后再决定集成

**6.** **[multica-ai/andrej-karpathy-skills](https://github.com/multica-ai/andrej-karpathy-skills)** — A single CLAUDE.md file to improve Claude Code behavior, derived from Andrej Karpathy's observations on LLM coding pitfalls.
`Stars: 170.4k` `未声明` `更新: 2026-04-20`

🏢 multica-ai（GitHub 组织账号） · 社区关注度高；由组织账号维护；近期仍有更新；便于沉淀为可复用 Agent 工作流；许可证不清，商用前需核实

**7.** **[farion1231/cc-switch](https://github.com/farion1231/cc-switch)** — 多种 Coding Agent 的桌面切换/管理工具
`Stars: 94.2k` `MIT` `更新: 2026-06-07`

🏢 farion1231（GitHub 个人/小团队账号） · 社区关注度高；由个人或小团队维护，迭代可能更灵活；许可证较清晰（MIT）；近期仍有更新；仍需阅读 README、Issue 和依赖清单后再决定集成

**8.** **[anthropics/claude-code](https://github.com/anthropics/claude-code)** — Anthropic 的终端 Coding Agent
`Stars: 130.9k` `未声明` `更新: 2026-06-06`

🏢 anthropics（GitHub 组织账号） · 社区关注度高；由组织账号维护；近期仍有更新；便于沉淀为可复用 Agent 工作流；许可证不清，商用前需核实

**9.** **[bytedance/deer-flow](https://github.com/bytedance/deer-flow)** — 字节开源长任务 SuperAgent 框架
`Stars: 70.7k` `MIT` `更新: 2026-06-08`

🏢 bytedance（GitHub 组织账号） · 社区关注度高；由组织账号维护；许可证较清晰（MIT）；近期仍有更新；仍需阅读 README、Issue 和依赖清单后再决定集成

**10.** **[paperclipai/paperclip](https://github.com/paperclipai/paperclip)** — 工作场景中的 Agent 管理平台
`Stars: 69.5k` `MIT` `更新: 2026-06-07`

🏢 paperclipai（GitHub 组织账号） · 社区关注度高；由组织账号维护；许可证较清晰（MIT）；近期仍有更新；仍需阅读 README、Issue 和依赖清单后再决定集成

**11.** **[earendil-works/pi](https://github.com/earendil-works/pi)** — 个人智能体/辅助工具项目
`Stars: 60.7k` `MIT` `更新: 2026-06-07`

🏢 earendil-works（GitHub 组织账号） · 社区关注度高；由组织账号维护；许可证较清晰（MIT）；近期仍有更新；仍需阅读 README、Issue 和依赖清单后再决定集成

**12.** **[ruvnet/ruflo](https://github.com/ruvnet/ruflo)** — 多智能体协同开发框架
`Stars: 58.4k` `MIT` `更新: 2026-06-07`

🏢 ruvnet（GitHub 个人/小团队账号） · 社区关注度高；由个人或小团队维护，迭代可能更灵活；许可证较清晰（MIT）；近期仍有更新；仍需阅读 README、Issue 和依赖清单后再决定集成

**13.** **[karpathy/autoresearch](https://github.com/karpathy/autoresearch)** — 单 GPU 自动研究 Agent 实验
`Stars: 85.5k` `未声明` `更新: 2026-03-26`

🏢 karpathy（GitHub 个人/小团队账号） · 社区关注度高；由个人或小团队维护，迭代可能更灵活；近期仍有更新；便于沉淀为可复用 Agent 工作流；许可证不清，商用前需核实

**14.** **[colbymchenry/codegraph](https://github.com/colbymchenry/codegraph)** — 代码图谱/代码理解项目
`Stars: 43.8k` `MIT` `更新: 2026-06-07`

🏢 colbymchenry（GitHub 个人/小团队账号） · 已有明显社区基础；由个人或小团队维护，迭代可能更灵活；许可证较清晰（MIT）；近期仍有更新；仍需阅读 README、Issue 和依赖清单后再决定集成

**15.** **[HKUDS/CLI-Anything](https://github.com/HKUDS/CLI-Anything)** — 把软件转为 Agent 可调用 CLI 的框架
`Stars: 42.3k` `Apache-2.0` `更新: 2026-06-04`

🏢 HKUDS（GitHub 组织账号） · 已有明显社区基础；由组织账号维护；许可证较清晰（Apache-2.0）；近期仍有更新；仍需阅读 README、Issue 和依赖清单后再决定集成

**16.** **[code-yeongyu/oh-my-openagent](https://github.com/code-yeongyu/oh-my-openagent)** — 多种 Agent 框架集合
`Stars: 61.4k` `NOASSERTION` `更新: 2026-06-07`

🏢 code-yeongyu（GitHub 个人/小团队账号） · 社区关注度高；由个人或小团队维护，迭代可能更灵活；近期仍有更新；便于沉淀为可复用 Agent 工作流；许可证不清，商用前需核实

**17.** **[tinyhumansai/openhuman](https://github.com/tinyhumansai/openhuman)** — 开源智能助手
`Stars: 31.1k` `GPL-3.0` `更新: 2026-06-07`

🏢 tinyhumansai（GitHub 组织账号） · 已有明显社区基础；由组织账号维护；许可证较清晰（GPL-3.0）；近期仍有更新；仍需阅读 README、Issue 和依赖清单后再决定集成

**18.** **[multica-ai/multica](https://github.com/multica-ai/multica)** — 多 Agent/产品化协作平台
`Stars: 35.7k` `NOASSERTION` `更新: 2026-06-07`

🏢 multica-ai（GitHub 组织账号） · 已有明显社区基础；由组织账号维护；近期仍有更新；便于沉淀为可复用 Agent 工作流；许可证不清，商用前需核实

**19.** **[AndyMik90/Aperant](https://github.com/AndyMik90/Aperant)** — 多会话自主编码 Agent
`Stars: 14.3k` `AGPL-3.0` `更新: 2026-03-23`

🏢 AndyMik90（GitHub 个人/小团队账号） · 已有明显社区基础；由个人或小团队维护，迭代可能更灵活；许可证较清晰（AGPL-3.0）；近期仍有更新；仍需阅读 README、Issue 和依赖清单后再决定集成

**20.** **[jnMetaCode/agency-agents-zh](https://github.com/jnMetaCode/agency-agents-zh)** — 中文专家 Agent 角色集合
`Stars: 14.2k` `MIT` `更新: 2026-06-03`

🏢 jnMetaCode（GitHub 个人/小团队账号） · 已有明显社区基础；由个人或小团队维护，迭代可能更灵活；许可证较清晰（MIT）；近期仍有更新；仍需阅读 README、Issue 和依赖清单后再决定集成

**21.** **[simular-ai/Agent-S](https://github.com/simular-ai/Agent-S)** — 面向 OSWorld 的通用电脑操作 Agent
`Stars: 11.8k` `Apache-2.0` `更新: 2026-05-13`

🏢 simular-ai（GitHub 组织账号） · 已有明显社区基础；由组织账号维护；许可证较清晰（Apache-2.0）；近期仍有更新；涉及肖像/声音合规和授权风险

**22.** **[datawhalechina/easy-vibe](https://github.com/datawhalechina/easy-vibe)** — Vibe Coding 教程与实践项目
`Stars: 16.5k` `未声明` `更新: 2026-06-03`

🏢 datawhalechina（GitHub 组织账号） · 已有明显社区基础；由组织账号维护；近期仍有更新；便于沉淀为可复用 Agent 工作流；许可证不清，商用前需核实

**23.** **[sirmalloc/ccstatusline](https://github.com/sirmalloc/ccstatusline)** — Claude Code 状态栏工具
`Stars: 10.3k` `MIT` `更新: 2026-06-02`

🏢 sirmalloc（GitHub 个人/小团队账号） · 已有明显社区基础；由个人或小团队维护，迭代可能更灵活；许可证较清晰（MIT）；近期仍有更新；仍需阅读 README、Issue 和依赖清单后再决定集成

**24.** **[HKUDS/OpenSpace](https://github.com/HKUDS/OpenSpace)** — 低成本、自进化 Agent 技能追踪优化项目
`Stars: 6.4k` `MIT` `更新: 2026-06-04`

🏢 HKUDS（GitHub 组织账号） · 已有明显社区基础；由组织账号维护；许可证较清晰（MIT）；近期仍有更新；仍需阅读 README、Issue 和依赖清单后再决定集成

**25.** **[HKUDS/ClawWork](https://github.com/HKUDS/ClawWork)** — OpenClaw AI 同事工作流
`Stars: 8.2k` `MIT` `更新: 2026-03-03`

🏢 HKUDS（GitHub 组织账号） · 已有明显社区基础；由组织账号维护；许可证较清晰（MIT）；近期仍有更新；仍需阅读 README、Issue 和依赖清单后再决定集成

**26.** **[TencentCloud/TencentDB-Agent-Memory](https://github.com/TencentCloud/TencentDB-Agent-Memory)** — 腾讯数据库 Agent 记忆项目
`Stars: 5.1k` `NOASSERTION` `更新: 2026-06-04`

🏢 TencentCloud（GitHub 组织账号） · 已有明显社区基础；由组织账号维护；近期仍有更新；便于沉淀为可复用 Agent 工作流；许可证不清，商用前需核实

**27.** **[datawhalechina/Agent-Learning-Hub](https://github.com/datawhalechina/Agent-Learning-Hub)** — Agent 学习与教程资料库
`Stars: 3.1k` `MIT` `更新: 2026-06-05`

🏢 datawhalechina（GitHub 组织账号） · 定位相对聚焦；由组织账号维护；许可证较清晰（MIT）；近期仍有更新；仍需阅读 README、Issue 和依赖清单后再决定集成

**28.** **[OpenBMB/PilotDeck](https://github.com/OpenBMB/PilotDeck)** — OpenBMB 的办公/Agent 工作台项目
`Stars: 3.0k` `AGPL-3.0` `更新: 2026-06-05`

🏢 OpenBMB（GitHub 组织账号） · 定位相对聚焦；由组织账号维护；许可证较清晰（AGPL-3.0）；近期仍有更新；仍需阅读 README、Issue 和依赖清单后再决定集成

**29.** **[iamzhihuix/skills-manage](https://github.com/iamzhihuix/skills-manage)** — 多平台 AI Coding Agent Skills 管理界面
`Stars: 2.0k` `Apache-2.0` `更新: 2026-05-02`

🏢 iamzhihuix（GitHub 个人/小团队账号） · 定位相对聚焦；由个人或小团队维护，迭代可能更灵活；许可证较清晰（Apache-2.0）；近期仍有更新；仍需阅读 README、Issue 和依赖清单后再决定集成

**30.** **[hesamsheikh/octogent](https://github.com/hesamsheikh/octogent)** — 多 Agent 协作开发工具
`Stars: 1.2k` `MIT` `更新: 2026-04-20`

🏢 hesamsheikh（GitHub 个人/小团队账号） · 定位相对聚焦；由个人或小团队维护，迭代可能更灵活；许可证较清晰（MIT）；近期仍有更新；仍需阅读 README、Issue 和依赖清单后再决定集成

**31.** **[clacky-ai/openclacky](https://github.com/clacky-ai/openclacky)** — 开源 AI 编程/开发工作台
`Stars: 942` `MIT` `更新: 2026-06-07`

🏢 clacky-ai（GitHub 组织账号） · 定位相对聚焦；由组织账号维护；许可证较清晰（MIT）；近期仍有更新；仍需阅读 README、Issue 和依赖清单后再决定集成

**32.** **[thunlp/ProactiveAgent](https://github.com/thunlp/ProactiveAgent)** — 主动式智能体研究项目
`Stars: 607` `Apache-2.0` `更新: 2026-05-12`

🏢 thunlp（GitHub 组织账号） · 定位相对聚焦；由组织账号维护；许可证较清晰（Apache-2.0）；近期仍有更新；仍需阅读 README、Issue 和依赖清单后再决定集成

**33.** **[xiaoyuanda666-ship-it/BaiLongma](https://github.com/xiaoyuanda666-ship-it/BaiLongma)** — 本地安装式 AI 助手/自动化项目
`Stars: 303` `MIT` `更新: 2026-06-07`

🏢 xiaoyuanda666-ship-it（GitHub 个人/小团队账号） · 定位相对聚焦；由个人或小团队维护，迭代可能更灵活；许可证较清晰（MIT）；近期仍有更新；社区验证样本偏少

**34.** **[googlecolab/google-colab-cli](https://github.com/googlecolab/google-colab-cli)** — Google Colab 命令行工具
`Stars: 146` `Apache-2.0` `更新: 2026-06-04`

🏢 googlecolab（GitHub 组织账号） · 定位相对聚焦；由组织账号维护；许可证较清晰（Apache-2.0）；近期仍有更新；社区验证样本偏少

**35.** **[WorldFlowAI/everything-claude-code](https://github.com/WorldFlowAI/everything-claude-code)** — Claude Code 资源与技巧集合
`Stars: 138` `未声明` `更新: 2026-01-23`

🏢 WorldFlowAI（GitHub 组织账号） · 定位相对聚焦；由组织账号维护；近期仍有更新；便于沉淀为可复用 Agent 工作流；许可证不清，商用前需核实；社区验证样本偏少

## 八、浏览器/桌面自动化与 Computer Use

**1.** **[pewdiepie-archdaemon/odysseus](https://github.com/pewdiepie-archdaemon/odysseus)** — 本地 AI 客户端/桌面应用项目
`Stars: 61.8k` `MIT` `更新: 2026-06-08`

🏢 pewdiepie-archdaemon（GitHub 个人/小团队账号） · 社区关注度高；由个人或小团队维护，迭代可能更灵活；许可证较清晰（MIT）；近期仍有更新；需要处理账号安全、权限隔离和反自动化限制

**2.** **[vercel-labs/agent-browser](https://github.com/vercel-labs/agent-browser)** — Vercel Labs 的 Agent 浏览器项目
`Stars: 35.5k` `Apache-2.0` `更新: 2026-06-05`

🏢 vercel-labs（GitHub 组织账号） · 已有明显社区基础；由组织账号维护；许可证较清晰（Apache-2.0）；近期仍有更新；需要处理账号安全、权限隔离和反自动化限制

**3.** **[CloakHQ/CloakBrowser](https://github.com/CloakHQ/CloakBrowser)** — 带反检测能力的 Chromium 自动化浏览器
`Stars: 24.7k` `MIT` `更新: 2026-06-07`

🏢 CloakHQ（GitHub 组织账号） · 已有明显社区基础；由组织账号维护；许可证较清晰（MIT）；近期仍有更新；需要处理账号安全、权限隔离和反自动化限制

**4.** **[trycua/cua](https://github.com/trycua/cua)** — 通用 Computer Use Agent 项目
`Stars: 17.7k` `MIT` `更新: 2026-06-05`

🏢 trycua（GitHub 组织账号） · 已有明显社区基础；由组织账号维护；许可证较清晰（MIT）；近期仍有更新；需要处理账号安全、权限隔离和反自动化限制

**5.** **[browser-use/browser-harness](https://github.com/browser-use/browser-harness)** — 浏览器自动化测试/执行框架
`Stars: 14.5k` `MIT` `更新: 2026-05-20`

🏢 browser-use（GitHub 组织账号） · 已有明显社区基础；由组织账号维护；许可证较清晰（MIT）；近期仍有更新；需要处理账号安全、权限隔离和反自动化限制

**6.** **[antirez/ds4](https://github.com/antirez/ds4)** — 小型原生推理引擎
`Stars: 13.2k` `MIT` `更新: 2026-06-06`

🏢 antirez（GitHub 个人/小团队账号） · 已有明显社区基础；由个人或小团队维护，迭代可能更灵活；许可证较清晰（MIT）；近期仍有更新；需要处理账号安全、权限隔离和反自动化限制

**7.** **[openclaw/Peekaboo](https://github.com/openclaw/Peekaboo)** — macOS 屏幕/窗口读取与自动化工具
`Stars: 4.7k` `MIT` `更新: 2026-06-07`

🏢 openclaw（GitHub 组织账号） · 定位相对聚焦；由组织账号维护；许可证较清晰（MIT）；近期仍有更新；需要处理账号安全、权限隔离和反自动化限制

**8.** **[TurixAI/TuriX-CUA](https://github.com/TurixAI/TuriX-CUA)** — 面向 Computer Use 的桌面/浏览器操作 Agent
`Stars: 3.0k` `MIT` `更新: 2026-06-03`

🏢 TurixAI（GitHub 组织账号） · 定位相对聚焦；由组织账号维护；许可证较清晰（MIT）；近期仍有更新；需要处理账号安全、权限隔离和反自动化限制

**9.** **[Mininglamp-AI/cider](https://github.com/Mininglamp-AI/cider)** — Mac AI 性能/运行优化工具
`Stars: 326` `MIT` `更新: 2026-06-05`

🏢 Mininglamp-AI（GitHub 组织账号） · 定位相对聚焦；由组织账号维护；许可证较清晰（MIT）；近期仍有更新；社区验证样本偏少；需要处理账号安全、权限隔离和反自动化限制

## 九、办公知识工作流与低代码自动化

**1.** **[n8n-io/n8n](https://github.com/n8n-io/n8n)** — 可自托管的低代码工作流自动化平台
`Stars: 191.5k` `NOASSERTION` `更新: 2026-06-08`

🏢 n8n-io（GitHub 组织账号） · 社区关注度高；由组织账号维护；近期仍有更新；许可证不清，商用前需核实

**2.** **[googleworkspace/cli](https://github.com/googleworkspace/cli)** — Google Workspace 命令行自动化工具
`Stars: 26.9k` `Apache-2.0` `更新: 2026-06-01`

🏢 googleworkspace（GitHub 组织账号） · 已有明显社区基础；由组织账号维护；许可证较清晰（Apache-2.0）；近期仍有更新；仍需阅读 README、Issue 和依赖清单后再决定集成

**3.** **[jackwener/OpenCLI](https://github.com/jackwener/OpenCLI)** — 通用 OpenCLI 工具
`Stars: 23.7k` `Apache-2.0` `更新: 2026-06-07`

🏢 jackwener（GitHub 个人/小团队账号） · 已有明显社区基础；由个人或小团队维护，迭代可能更灵活；许可证较清晰（Apache-2.0）；近期仍有更新；仍需阅读 README、Issue 和依赖清单后再决定集成

**4.** **[lewislulu/html-ppt-skill](https://github.com/lewislulu/html-ppt-skill)** — HTML/PPT 生成 Skill
`Stars: 5.7k` `MIT` `更新: 2026-04-26`

🏢 lewislulu（GitHub 个人/小团队账号） · 已有明显社区基础；由个人或小团队维护，迭代可能更灵活；许可证较清晰（MIT）；近期仍有更新；仍需阅读 README、Issue 和依赖清单后再决定集成

**5.** **[jackwener/wx-cli](https://github.com/jackwener/wx-cli)** — 微信 CLI 工具
`Stars: 3.3k` `Apache-2.0` `更新: 2026-05-19`

🏢 jackwener（GitHub 个人/小团队账号） · 定位相对聚焦；由个人或小团队维护，迭代可能更灵活；许可证较清晰（Apache-2.0）；近期仍有更新；仍需阅读 README、Issue 和依赖清单后再决定集成

**6.** **[huohuoer/wechat-cli](https://github.com/huohuoer/wechat-cli)** — 微信 CLI 工具
`Stars: 1.3k` `Apache-2.0` `更新: 2026-04-06`

🏢 huohuoer（GitHub 个人/小团队账号） · 定位相对聚焦；由个人或小团队维护，迭代可能更灵活；许可证较清晰（Apache-2.0）；近期仍有更新；仍需阅读 README、Issue 和依赖清单后再决定集成

**7.** **[zarazhangrui/lark-coding-agent-bridge](https://github.com/zarazhangrui/lark-coding-agent-bridge)** — 飞书与 Claude Code 的桥接工具
`Stars: 1.0k` `MIT` `更新: 2026-06-04`

🏢 zarazhangrui（GitHub 个人/小团队账号） · 定位相对聚焦；由个人或小团队维护，迭代可能更灵活；许可证较清晰（MIT）；近期仍有更新；仍需阅读 README、Issue 和依赖清单后再决定集成

**8.** **[paperclipai/companies](https://github.com/paperclipai/companies)** — AI 公司/组织资料库
`Stars: 685` `未声明` `更新: 2026-03-23`

🏢 paperclipai（GitHub 组织账号） · 定位相对聚焦；由组织账号维护；近期仍有更新；许可证不清，商用前需核实

**9.** **[Tencent/openclaw-weixin](https://github.com/Tencent/openclaw-weixin)** — 微信与 OpenClaw 连接插件
`Stars: 567` `NOASSERTION` `更新: 2026-05-18`

🏢 Tencent（GitHub 组织账号） · 定位相对聚焦；由组织账号维护；近期仍有更新；许可证不清，商用前需核实

**10.** **[nicepkg/auto-company](https://github.com/nicepkg/auto-company)** — 自动化公司/一人公司工具项目
`Stars: 161` `未声明` `更新: 2026-02-12`

🏢 nicepkg（GitHub 组织账号） · 定位相对聚焦；由组织账号维护；近期仍有更新；许可证不清，商用前需核实；社区验证样本偏少

## 十、AI Skills、Prompt 与方法论资产

**1.** **[mattpocock/skills](https://github.com/mattpocock/skills)** — 工程师实践型 Skills 集合
`Stars: 120.5k` `MIT` `更新: 2026-06-07`

🏢 mattpocock（GitHub 个人/小团队账号） · 社区关注度高；由个人或小团队维护，迭代可能更灵活；许可证较清晰（MIT）；近期仍有更新；多数是资产/方法论，不是可直接运行的完整产品

**2.** **[garrytan/gstack](https://github.com/garrytan/gstack)** — 面向一人公司/团队角色模拟的 Claude Code 配置
`Stars: 108.1k` `MIT` `更新: 2026-06-08`

🏢 garrytan（GitHub 个人/小团队账号） · 社区关注度高；由个人或小团队维护，迭代可能更灵活；许可证较清晰（MIT）；近期仍有更新；多数是资产/方法论，不是可直接运行的完整产品

**3.** **[anthropics/skills](https://github.com/anthropics/skills)** — Anthropic 官方 Agent Skills 仓库
`Stars: 147.6k` `未声明` `更新: 2026-06-07`

🏢 anthropics（GitHub 组织账号） · 社区关注度高；由组织账号维护；近期仍有更新；便于沉淀为可复用 Agent 工作流；许可证不清，商用前需核实；多数是资产/方法论，不是可直接运行的完整产品

**4.** **[dair-ai/Prompt-Engineering-Guide](https://github.com/dair-ai/Prompt-Engineering-Guide)** — 提示工程与上下文工程资料库
`Stars: 75.4k` `MIT` `更新: 2026-03-11`

🏢 dair-ai（GitHub 组织账号） · 社区关注度高；由组织账号维护；许可证较清晰（MIT）；近期仍有更新；多数是资产/方法论，不是可直接运行的完整产品

**5.** **[addyosmani/agent-skills](https://github.com/addyosmani/agent-skills)** — Addy Osmani 的 Agent Skills 集合
`Stars: 49.0k` `MIT` `更新: 2026-06-07`

🏢 addyosmani（GitHub 个人/小团队账号） · 已有明显社区基础；由个人或小团队维护，迭代可能更灵活；许可证较清晰（MIT）；近期仍有更新；多数是资产/方法论，不是可直接运行的完整产品

**6.** **[kepano/obsidian-skills](https://github.com/kepano/obsidian-skills)** — Obsidian 相关 Skills
`Stars: 34.8k` `MIT` `更新: 2026-06-08`

🏢 kepano（GitHub 个人/小团队账号） · 已有明显社区基础；由个人或小团队维护，迭代可能更灵活；许可证较清晰（MIT）；近期仍有更新；多数是资产/方法论，不是可直接运行的完整产品

**7.** **[coreyhaines31/marketingskills](https://github.com/coreyhaines31/marketingskills)** — 营销和副业方向 Skills
`Stars: 32.3k` `MIT` `更新: 2026-06-05`

🏢 coreyhaines31（GitHub 个人/小团队账号） · 已有明显社区基础；由个人或小团队维护，迭代可能更灵活；许可证较清晰（MIT）；近期仍有更新；多数是资产/方法论，不是可直接运行的完整产品

**8.** **[FujiwaraChoki/MoneyPrinterV2](https://github.com/FujiwaraChoki/MoneyPrinterV2)** — 自动化在线变现流程工具
`Stars: 30.8k` `AGPL-3.0` `更新: 2026-05-15`

🏢 FujiwaraChoki（GitHub 个人/小团队账号） · 已有明显社区基础；由个人或小团队维护，迭代可能更灵活；许可证较清晰（AGPL-3.0）；近期仍有更新；多数是资产/方法论，不是可直接运行的完整产品

**9.** **[davila7/claude-code-templates](https://github.com/davila7/claude-code-templates)** — Claude Code 模板与 Skill 工具集
`Stars: 27.8k` `MIT` `更新: 2026-06-07`

🏢 davila7（GitHub 个人/小团队账号） · 已有明显社区基础；由个人或小团队维护，迭代可能更灵活；许可证较清晰（MIT）；近期仍有更新；多数是资产/方法论，不是可直接运行的完整产品

**10.** **[K-Dense-AI/scientific-agent-skills](https://github.com/K-Dense-AI/scientific-agent-skills)** — 科研、论文写作和深度内容 Skills
`Stars: 27.5k` `MIT` `更新: 2026-06-07`

🏢 K-Dense-AI（GitHub 组织账号） · 已有明显社区基础；由组织账号维护；许可证较清晰（MIT）；近期仍有更新；多数是资产/方法论，不是可直接运行的完整产品

**11.** **[Donchitos/Claude-Code-Game-Studios](https://github.com/Donchitos/Claude-Code-Game-Studios)** — 游戏开发 Agent Studio 配置
`Stars: 21.1k` `MIT` `更新: 2026-05-21`

🏢 Donchitos（GitHub 个人/小团队账号） · 已有明显社区基础；由个人或小团队维护，迭代可能更灵活；许可证较清晰（MIT）；近期仍有更新；多数是资产/方法论，不是可直接运行的完整产品

**12.** **[EveryInc/compound-engineering-plugin](https://github.com/EveryInc/compound-engineering-plugin)** — 长期内容/产品运营相关插件
`Stars: 20.4k` `MIT` `更新: 2026-06-07`

🏢 EveryInc（GitHub 组织账号） · 已有明显社区基础；由组织账号维护；许可证较清晰（MIT）；近期仍有更新；多数是资产/方法论，不是可直接运行的完整产品

**13.** **[linshenkx/prompt-optimizer](https://github.com/linshenkx/prompt-optimizer)** — 提示词优化器
`Stars: 30.6k` `NOASSERTION` `更新: 2026-06-02`

🏢 linshenkx（GitHub 个人/小团队账号） · 已有明显社区基础；由个人或小团队维护，迭代可能更灵活；近期仍有更新；便于沉淀为可复用 Agent 工作流；许可证不清，商用前需核实；多数是资产/方法论，不是可直接运行的完整产品

**14.** **[vercel-labs/skills](https://github.com/vercel-labs/skills)** — Vercel Labs Skills 仓库
`Stars: 21.6k` `未声明` `更新: 2026-06-05`

🏢 vercel-labs（GitHub 组织账号） · 已有明显社区基础；由组织账号维护；近期仍有更新；便于沉淀为可复用 Agent 工作流；许可证不清，商用前需核实；多数是资产/方法论，不是可直接运行的完整产品

**15.** **[MiniMax-AI/skills](https://github.com/MiniMax-AI/skills)** — MiniMax 官方/社区 Skills 集合
`Stars: 12.4k` `MIT` `更新: 2026-04-18`

🏢 MiniMax-AI（GitHub 组织账号） · 已有明显社区基础；由组织账号维护；许可证较清晰（MIT）；近期仍有更新；多数是资产/方法论，不是可直接运行的完整产品

**16.** **[easychen/opc-methodology](https://github.com/easychen/opc-methodology)** — 一人企业方法论
`Stars: 16.0k` `NOASSERTION` `更新: 2026-04-23`

🏢 easychen（GitHub 个人/小团队账号） · 已有明显社区基础；由个人或小团队维护，迭代可能更灵活；近期仍有更新；便于沉淀为可复用 Agent 工作流；许可证不清，商用前需核实；多数是资产/方法论，不是可直接运行的完整产品

**17.** **[virgiliojr94/book-to-skill](https://github.com/virgiliojr94/book-to-skill)** — 把书转换为 Skills 的工具
`Stars: 4.6k` `MIT` `更新: 2026-06-07`

🏢 virgiliojr94（GitHub 个人/小团队账号） · 定位相对聚焦；由个人或小团队维护，迭代可能更灵活；许可证较清晰（MIT）；近期仍有更新；多数是资产/方法论，不是可直接运行的完整产品

**18.** **[bleedline/aimoneyhunter](https://github.com/bleedline/aimoneyhunter)** — AI 赚钱/副业项目集合
`Stars: 17.3k` `未声明` `更新: 2025-10-20`

🏢 bleedline（GitHub 个人/小团队账号） · 已有明显社区基础；由个人或小团队维护，迭代可能更灵活；便于沉淀为可复用 Agent 工作流；许可证不清，商用前需核实；多数是资产/方法论，不是可直接运行的完整产品

**19.** **[nicedreamzapp/claude-code-local](https://github.com/nicedreamzapp/claude-code-local)** — Claude Code 本地化/大模型运行相关项目
`Stars: 2.7k` `MIT` `更新: 2026-06-05`

🏢 nicedreamzapp（GitHub 个人/小团队账号） · 定位相对聚焦；由个人或小团队维护，迭代可能更灵活；许可证较清晰（MIT）；近期仍有更新；涉及肖像/声音合规和授权风险；多数是资产/方法论，不是可直接运行的完整产品

**20.** **[XiaomingX/ai-money-maker-handbook](https://github.com/XiaomingX/ai-money-maker-handbook)** — AI 副业赚钱手册
`Stars: 2.6k` `Apache-2.0` `更新: 2026-06-07`

🏢 XiaomingX（GitHub 个人/小团队账号） · 定位相对聚焦；由个人或小团队维护，迭代可能更灵活；许可证较清晰（Apache-2.0）；近期仍有更新；多数是资产/方法论，不是可直接运行的完整产品

**21.** **[kangarooking/cangjie-skill](https://github.com/kangarooking/cangjie-skill)** — 把书籍方法论沉淀为可调用 Skill
`Stars: 1.1k` `MIT` `更新: 2026-06-03`

🏢 kangarooking（GitHub 个人/小团队账号） · 定位相对聚焦；由个人或小团队维护，迭代可能更灵活；许可证较清晰（MIT）；近期仍有更新；多数是资产/方法论，不是可直接运行的完整产品

**22.** **[binggandata/bggg-skills](https://github.com/binggandata/bggg-skills)** — Skill 自我优化/饕餮 Skill 项目
`Stars: 378` `MIT` `更新: 2026-05-05`

🏢 binggandata（GitHub 个人/小团队账号） · 定位相对聚焦；由个人或小团队维护，迭代可能更灵活；许可证较清晰（MIT）；近期仍有更新；社区验证样本偏少；多数是资产/方法论，不是可直接运行的完整产品

**23.** **[clawvader-tech/hermes-telegram-miniapp](https://github.com/clawvader-tech/hermes-telegram-miniapp)** — Telegram 内远程终端控制面板
`Stars: 233` `MIT` `更新: 2026-04-15`

🏢 clawvader-tech（GitHub 个人/小团队账号） · 定位相对聚焦；由个人或小团队维护，迭代可能更灵活；许可证较清晰（MIT）；近期仍有更新；社区验证样本偏少；多数是资产/方法论，不是可直接运行的完整产品

**24.** **[AndrewNgGirl/SkillLens](https://github.com/AndrewNgGirl/SkillLens)** — Agent Skill 评测与改进建议工具
`Stars: 60` `MIT` `更新: 2026-05-17`

🏢 AndrewNgGirl（GitHub 个人/小团队账号） · 定位相对聚焦；由个人或小团队维护，迭代可能更灵活；许可证较清晰（MIT）；近期仍有更新；社区验证样本偏少；多数是资产/方法论，不是可直接运行的完整产品

## 十一、其他工具、数据源与垂直实验

**1.** **[public-apis/public-apis](https://github.com/public-apis/public-apis)** — 免费公共 API 集合
`Stars: 440.0k` `MIT` `更新: 2026-06-07`

🏢 public-apis（GitHub 组织账号） · 社区关注度高；由组织账号维护；许可证较清晰（MIT）；近期仍有更新；仍需阅读 README、Issue 和依赖清单后再决定集成

**2.** **[DestinyLinker/MingLi-Bench](https://github.com/DestinyLinker/MingLi-Bench)** — 中文命理任务 LLM 评测基准
`Stars: 1.6k` `MIT` `更新: 2026-05-09`

🏢 DestinyLinker（GitHub 组织账号） · 定位相对聚焦；由组织账号维护；许可证较清晰（MIT）；近期仍有更新；仍需阅读 README、Issue 和依赖清单后再决定集成

## 十二、非仓库或不可访问 GitHub 入口

**1.** **[NVIDIA/DanceDiffusion](https://github.com/NVIDIA)** — 原清单中的 DanceDiffusion 指向已不可作为仓库访问
`非仓库/不可访问；来源行：37；原分类：视频`

🏢 NVIDIA（Organization） · 可作为入口追踪相关团队或产品线；未指向单一仓库，无法直接评估代码、许可证、依赖和维护状态

**2.** **[YadiraF/ClothFlow](https://github.com/YadiraF)** — 原清单中的 ClothFlow 指向已不可作为仓库访问
`非仓库/不可访问；来源行：44；原分类：视频`

🏢 YadiraF（Organization） · 可作为入口追踪相关团队或产品线；未指向单一仓库，无法直接评估代码、许可证、依赖和维护状态

**3.** **[TauricResearch](https://github.com/TauricResearch)** — 围绕 TauricResearch 的开源项目
`非仓库/不可访问；来源行：141；原分类：金融`

🏢 TauricResearch（Organization） · 可作为入口追踪相关团队或产品线；未指向单一仓库，无法直接评估代码、许可证、依赖和维护状态

**4.** **[ghuntley](https://github.com/ghuntley)** — 围绕 ghuntley 的开源项目
`非仓库/不可访问；来源行：310；原分类：其他`

🏢 ghuntley（User） · 可作为入口追踪相关团队或产品线；未指向单一仓库，无法直接评估代码、许可证、依赖和维护状态

**5.** **[features/copilot](https://github.com/features/copilot)** — GitHub Copilot 产品入口，不是仓库
`非仓库/不可访问；来源行：272；原分类：编程 & Agent`

🏢 未能从 GitHub 仓库接口确认 · 可作为入口追踪相关团队或产品线；未指向单一仓库，无法直接评估代码、许可证、依赖和维护状态

**6.** **[binance](https://github.com/binance)** — 围绕 binance 的开源项目
`非仓库/不可访问；来源行：147；原分类：金融`

🏢 binance（Organization） · 可作为入口追踪相关团队或产品线；未指向单一仓库，无法直接评估代码、许可证、依赖和维护状态

## 十三、官网 / 产品页 / 非 GitHub 入口

这些链接不是可直接评估的单一 GitHub 仓库，建议只作为产品或组织入口，再按具体仓库、价格、许可和数据合规单独确认。

**1.** **[OpenToonz 官网](https://opentoonz.github.io/e/index.html)** — 开源二维动画软件入口
`页面入口`

OpenToonz 官网，不是 GitHub 仓库链接

**2.** **[万镜一刻](https://www.yikeai.com/#/home)** — 阿里云 AI 视频平台入口
`页面入口`

阿里云“万镜一刻”入口，需官网确认开放性和价格

**3.** **[Wind 金融技能页](https://aifinmarket.wind.com.cn/skill.md)** — Wind 金融 Skill 文档入口
`页面入口`

Wind 金融 Skill 文档入口，非 GitHub 仓库

**4.** **[BeeQuant](https://beequant.io/home)** — BeeQuant 官网入口
`页面入口`

BeeQuant 官网入口，需确认产品形态

**5.** **[AlphaGBM](https://www.alphagbm.com/)** — AlphaGBM 官网入口
`页面入口`

AlphaGBM 官网入口，GitHub 仓库另有 AlphaGBM/skills

**6.** **[getdesign.md](https://getdesign.md/)** — awesome-design-md 配套站点
`页面入口`

awesome-design-md 配套站点

**7.** **[MCPMarket UI Prompt Generator](https://mcpmarket.com/zh/tools/skills/ui-prompt-generator)** — UI 提示工具页
`页面入口`

MCP 市场工具页，非 GitHub 仓库

**8.** **[腾讯 ArDot](https://ardot.tencent.com/)** — 腾讯设计平台入口
`页面入口`

腾讯 Ardot 官网入口

**9.** **[QoderWake](https://qoder.com/qoderwake)** — 阿里 QoderWake 数字员工入口
`页面入口`

阿里 QoderWake 产品入口

**10.** **[Marvis](https://marvis.qq.com/)** — 腾讯系统级助手入口
`页面入口`

腾讯 Marvis 产品入口

**11.** **[CodeBuddy Work Buddy](https://www.codebuddy.cn/work/)** — 腾讯 Work Buddy 产品入口
`页面入口`

腾讯 Work Buddy 产品入口

**12.** **[Clockless AI](https://clockless.ai/)** — 客户关系 AI 门户
`页面入口`

商业 AI 同事/客户管家入口

**13.** **[Helio](https://www.helio.im/)** — AI 原生团队工作区
`页面入口`

商业 AI 同事入口

**14.** **[Datawhale easy-vibe 文档](https://datawhalechina.github.io/easy-vibe/zh-cn/)** — Vibe Coding 教程站
`页面入口`

Datawhale easy-vibe 文档站，GitHub 仓库另有 datawhalechina/easy-vibe

**15.** **[PilotDeck](https://pilotdeck.openbmb.cn/pilotdeck.github.io/)** — OpenBMB PilotDeck 官网入口
`页面入口`

PilotDeck 官网入口，GitHub 仓库另有 OpenBMB/PilotDeck

**16.** **[ClawinLink](https://claw.baolieguoshi.com/)** — Agent 消息网关入口
`页面入口`

ClawinLink 官网入口，非 GitHub 仓库

## 十四、注意事项

**换脸、人脸识别、声音克隆、数字人、桌面控制、浏览器控制、微信/QQ/小红书通道**
`涉及隐私、账号、平台规则和误操作风险`

必须做权限隔离、日志审计、人工确认、素材授权和合规边界。

**金融交易 Agent / 交易所 SDK**
`容易被误用为实盘自动交易`

先做研究、回测、模拟盘；实盘需要风控和合规审查。

**Skills / Prompt / Awesome 类仓库**
`多数是方法论或素材资产，不是完整应用`

适合迁移成自己的本地 Skill，统一入口、输出格式和验收脚本。

## 联系方式

| 个人微信 | 公众号 |
|:---:|:---:|
| <img src="./wechat.jpg" width="200" /> | <img src="./gzh.png" width="200" /> |
| 扫码添加微信 | 扫码关注公众号 |
