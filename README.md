# 165个 GitHub AI / Agent 仓库分类推荐清单

GitHub AI / Agent 仓库分类推荐清单，覆盖图片生成、语音识别、视频自动化、金融研究、Agent 编程、浏览器自动化等方向。

生成时间：2026-05-26（Asia/Shanghai）

数据来源：原始两份分析文档、GitHub REST API、仓库 README/常见依赖文件探测；非 GitHub 链接仅做入口级判断。GitHub 的 `pushed_at` / 最后提交时间以原文档记录为准，日期口径可能包含 UTC 与 CST 差异。

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
| 本地图片生成工作流 | ComfyUI、Stable Diffusion WebUI、Diffusers | 生态成熟，可扩展性强 |
| 图片增强/修复 | Real-ESRGAN、GFPGAN、Segment Anything、GroundingDINO | 可作为生成前后处理模块 |
| 人脸识别/换脸 | DeepFace、FaceFusion、Deep-Live-Cam | 工具成熟，但要注意合规和授权 |
| 语音识别 | Whisper、whisper.cpp、NeMo、ESPnet | 稳定、生态广，适合本地或服务端 |
| 中文语音生成 | VoxCPM、Piper、Bark、Coqui TTS | 中文生成和本地 TTS 可组合验证 |
| 视频生成/自动化 | MoneyPrinterTurbo、Remotion、HyperFrames、MoviePy、FFmpeg | 从短视频自动化到工程化渲染都有覆盖 |
| 自媒体采集与生产 | yt-dlp、Firecrawl、Scrapling、browser-use、MoneyPrinterTurbo | 覆盖采集、清洗、浏览器自动化、生成 |
| 金融研究/回测 | OpenBB、Qlib、vn.py、Backtrader、TradingAgents | 研究和回测优先，实盘需谨慎 |
| 设计系统/组件 | shadcn-ui、Ant Design、MUI、Storybook、Tailwind CSS | 组件和工程生态强 |
| Agent 编程工作流 | Codex、OpenHands、deer-flow、OpenClaw、AutoGen、LangGraph | 覆盖 CLI、软件工程、多 Agent 编排 |
| Agent 技能资产 | anthropics/skills、superpowers、agent-skills、MiniMax-AI/skills | 适合沉淀工作流和提示资产 |
| 浏览器/桌面自动化 | agent-s、TuriX-CUA、browser-use、Playwright、Peekaboo | 要做权限隔离、日志审计和账号风控 |

## 一、图片

**1.** **[Comfy-Org/ComfyUI](https://github.com/Comfy-Org/ComfyUI)** — 节点式生成工作流
`Stars: 114.6k` `GPL-3.0；代码免费开源` `更新: 2026-05-26`

🏢 Comfy Org · 本地图片工作流首选，生态强；部署和显存成本较高

**2.** **[AUTOMATIC1111/stable-diffusion-webui](https://github.com/AUTOMATIC1111/stable-diffusion-webui)** — SD 网页生成界面
`Stars: 163.3k` `AGPL-3.0` `更新: 2026-03-02`

🏢 AUTOMATIC1111 · 插件和资料最多；AGPL 商业复用要谨慎

**3.** **[huggingface/diffusers](https://github.com/huggingface/diffusers)** — 扩散模型库
`Stars: 33.7k` `Apache-2.0` `更新: 2026-05-26`

🏢 Hugging Face · 工程化调用模型更合适；需要自己搭 UI/流程

**4.** **[facebookresearch/segment-anything](https://github.com/facebookresearch/segment-anything)** — 图像分割模型
`Stars: 54.2k` `Apache-2.0` `更新: 2024-09-18`

🏢 Meta · 抠图/分割基础能力强；模型和算力另算

**5.** **[lllyasviel/ControlNet](https://github.com/lllyasviel/ControlNet)** — 可控图像生成
`Stars: 33.9k` `Apache-2.0` `更新: 2024-02-25`

🏢 lllyasviel · 姿态/边缘/深度控制经典方案；维护节奏偏旧

**6.** **[xinntao/Real-ESRGAN](https://github.com/xinntao/Real-ESRGAN)** — 图像视频超分
`Stars: 35.6k` `BSD-3-Clause` `更新: 2024-08-06`

🏢 Xintao · 图片/视频增强实用；更新偏旧但仍常用

**7.** **[TencentARC/GFPGAN](https://github.com/TencentARC/GFPGAN)** — 人脸修复增强
`Stars: 37.5k` `NOASSERTION` `更新: 2024-07-26`

🏢 腾讯 ARC Lab · 人脸修复效果好；许可证不清需核实

**8.** **[serengil/deepface](https://github.com/serengil/deepface)** — 人脸识别分析库
`Stars: 22.8k` `MIT；代码免费开源` `更新: 2026-05-13`

🏢 Sefik Serengil · 人脸识别/分析成熟；涉及隐私合规

**9.** **[facefusion/facefusion](https://github.com/facefusion/facefusion)** — 人脸融合工具
`Stars: 28.4k` `NOASSERTION；仓库免费` `更新: 2026-05-26`

🏢 FaceFusion · 活跃、可落地；换脸场景需合规审查

**10.** **[lllyasviel/Fooocus](https://github.com/lllyasviel/Fooocus)** — 轻量图像生成
`Stars: 49.0k` `GPL-3.0` `更新: 2025-12-01`

🏢 lllyasviel · 上手简单；扩展性不如 ComfyUI

**11.** **[Stability-AI/generative-models](https://github.com/Stability-AI/generative-models)** — 扩散模型代码
`Stars: 27.2k` `MIT` `更新: 2025-12-16`

🏢 Stability AI · 适合研究模型本体；落地需工程封装

**12.** **[IDEA-Research/GroundingDINO](https://github.com/IDEA-Research/GroundingDINO)** — 开放词检测
`Stars: 10.2k` `Apache-2.0` `更新: 2024-08-12`

🏢 IDEA Research · 与 SAM/自动标注组合价值高；部署成本较高

**13.** **[antvis/Infographic](https://github.com/antvis/Infographic)** — AI 信息图生成渲染框架
`Stars: 5.1k` `MIT；代码免费开源` `更新: 2026-05-06`

🏢 蚂蚁 AntV · AI 驱动的信息图生成渲染框架

**14.** **[EvoLinkAI/awesome-gpt-image-2-API-and-Prompts](https://github.com/EvoLinkAI/awesome-gpt-image-2-API-and-Prompts)** — 图像 API 提示集
`Stars: 15.6k` `CC0-1.0` `更新: 2026-05-22`

🏢 EvoLinkAI · 提示词积累有价值；依赖具体模型效果

**15.** **[freestylefly/awesome-gpt-image-2](https://github.com/freestylefly/awesome-gpt-image-2)** — 图像提示资源库
`Stars: 6.6k` `MIT` `更新: 2026-05-25`

🏢 苍何 · 适合做提示素材库；不是生产工具

**16.** **[YouMind-OpenLab/awesome-gpt-image-2](https://github.com/YouMind-OpenLab/awesome-gpt-image-2)** — GPT 图像提示集
`Stars: 6.7k` `NOASSERTION` `更新: 2026-05-26`

🏢 YouMind OpenLab · 活跃；许可证不清

**17.** **[YouMind-OpenLab/awesome-nano-banana-pro-prompts](https://github.com/YouMind-OpenLab/awesome-nano-banana-pro-prompts)** — Gemini 图像生成提示词库
`Stars: 12.2k` `NOASSERTION` `更新: 2026-05-26`

🏢 YouMind OpenLab · Google Gemini 图像生成提示词 10000+；许可证不清

**18.** **[JimLiu/baoyu-skills](https://github.com/JimLiu/baoyu-skills)** — 宝玉技能合集
`Stars: 19.6k` `未声明` `更新: 2026-05-26`

🏢 宝玉 · 技能资产可参考；复用需确认授权


## 二、语音

**1.** **[openai/whisper](https://github.com/openai/whisper)** — 通用语音识别
`Stars: 100.6k` `MIT；代码免费；API 可能收费` `更新: 2026-04-15`

🏢 OpenAI · ASR 首选基线，生态广

**2.** **[ggml-org/whisper.cpp](https://github.com/ggml-org/whisper.cpp)** — 本地 Whisper 推理
`Stars: 50.2k` `MIT` `更新: 2026-05-26`

🏢 ggml · 本地低成本部署优秀；功能聚焦推理

**3.** **[NVIDIA-NeMo/NeMo](https://github.com/NVIDIA-NeMo/NeMo)** — LLM/语音/多模态 AI 框架
`Stars: 17.3k` `Apache-2.0` `更新: 2026-05-26`

🏢 NVIDIA · 企业级 LLM/语音/多模态框架；部署较重

**4.** **[espnet/espnet](https://github.com/espnet/espnet)** — 端到端语音套件
`Stars: 9.8k` `Apache-2.0` `更新: 2026-05-25`

🏢 ESPnet · 研究和训练能力强；上手成本高

**5.** **[OpenBMB/VoxCPM](https://github.com/OpenBMB/VoxCPM)** — 多语言 TTS 与声音克隆
`Stars: 19.9k` `Apache-2.0` `更新: 2026-05-22`

🏢 清华/面壁智能 · 多语言 TTS + 声音设计 + 声音克隆；模型资源另算

**6.** **[rhasspy/piper](https://github.com/rhasspy/piper)** — 本地 TTS 系统
`Stars: 11.0k` `MIT` `更新: 2025-08-26`

🏢 Rhasspy · 本地 TTS 轻量实用；音色质量需实测

**7.** **[suno-ai/bark](https://github.com/suno-ai/bark)** — 生成式语音模型
`Stars: 39.1k` `MIT` `更新: 2024-08-19`

🏢 Suno · 生成能力强；维护偏旧

**8.** **[coqui-ai/TTS](https://github.com/coqui-ai/TTS)** — 开源 TTS 工具箱
`Stars: 45.4k` `MPL-2.0` `更新: 2024-08-16`

🏢 Coqui · 星标高、功能全；维护偏旧

**9.** **[snakers4/silero-models](https://github.com/snakers4/silero-models)** — 轻量预训练 TTS 模型
`Stars: 5.9k` `NOASSERTION` `更新: 2026-05-20`

🏢 Silero · 轻量模型适合边缘验证；授权需核实

**10.** **[microsoft/SpeechT5](https://github.com/microsoft/SpeechT5)** — 语音文本预训练
`Stars: 1.4k` `MIT` `更新: 2024-04-24`

🏢 微软 · 研究参考价值高；更新偏旧

**11.** **[abus-aikorea/voice-pro](https://github.com/abus-aikorea/voice-pro)** — TTS/语音克隆/音频处理工作台
`Stars: 10.3k` `GPL-3.0` `更新: 2025-12-05`

🏢 ABUS · 集成 TTS/声音克隆/Whisper/人声分离/翻译；需实测稳定性

**12.** **[mozilla/DeepSpeech](https://github.com/mozilla/DeepSpeech)** — 离线语音识别
`Stars: 26.8k` `MPL-2.0` `更新: 2025-06-19`

🏢 Mozilla · 历史项目参考；新项目优先 Whisper 系


## 三、视频

**1.** **[FFmpeg/FFmpeg](https://github.com/FFmpeg/FFmpeg)** — 音视频处理核心
`Stars: 60.5k` `NOASSERTION` `更新: 2026-05-26`

🏢 FFmpeg · 所有视频自动化底座；许可证细节需按组件核实

**2.** **[remotion-dev/remotion](https://github.com/remotion-dev/remotion)** — React 生成视频
`Stars: 48.1k` `NOASSERTION` `更新: 2026-05-26`

🏢 Remotion · 工程化视频渲染强；商业授权需核实

**3.** **[heygen-com/hyperframes](https://github.com/heygen-com/hyperframes)** — HTML 视频生成框架
`Stars: 21.5k` `Apache-2.0` `更新: 2026-05-26`

🏢 HeyGen · 适合代码化视频、字幕、动画

**4.** **[harry0703/MoneyPrinterTurbo](https://github.com/harry0703/MoneyPrinterTurbo)** — 一键短视频生成
`Stars: 59.8k` `MIT` `更新: 2026-05-26`

🏢 Harry · 短视频自动化最值得先看；API/素材/平台成本另算

**5.** **[Zulko/moviepy](https://github.com/Zulko/moviepy)** — Python 视频剪辑
`Stars: 14.6k` `MIT` `更新: 2026-03-07`

🏢 Zulko · Python 自动剪辑实用；复杂渲染不如 Remotion

**6.** **[mifi/lossless-cut](https://github.com/mifi/lossless-cut)** — 无损视频剪切
`Stars: 40.7k` `GPL-2.0` `更新: 2026-05-23`

🏢 Mikael Finstad · 素材切割非常实用；不是生成框架

**7.** **[obsproject/obs-studio](https://github.com/obsproject/obs-studio)** — 直播录屏软件
`Stars: 72.7k` `GPL-2.0` `更新: 2026-05-23`

🏢 OBS Project · 录制/直播基础能力强；二开成本高

**8.** **[hacksider/Deep-Live-Cam](https://github.com/hacksider/Deep-Live-Cam)** — 实时换脸工具
`Stars: 93.4k` `AGPL-3.0` `更新: 2026-05-24`

🏢 hacksider · 社区强、活跃；换脸合规和 AGPL 风险高

**9.** **[AIDC-AI/Pixelle-Video](https://github.com/AIDC-AI/Pixelle-Video)** — AI 全自动短视频引擎
`Stars: 20.0k` `Apache-2.0` `更新: 2026-05-18`

🏢 AIDC-AI · 全自动短视频引擎；部署成本高

**10.** **[MemeCalculate/moyin-creator](https://github.com/MemeCalculate/moyin-creator)** — AI 影视生产级工具
`Stars: 3.7k` `AGPL-3.0` `更新: 2026-05-25`

🏢 MemeCalculate · 支持 Seedance 2.0 / 剧本到成片全流程；AGPL 商用限制

**11.** **[elebumm/RedditVideoMakerBot](https://github.com/elebumm/RedditVideoMakerBot)** — Reddit 视频生成
`Stars: 12.3k` `GPL-3.0` `更新: 2026-05-25`

🏢 Lewis Menelaws · 自动化链路成熟；内容平台规则风险

**12.** **[opentoonz/opentoonz](https://github.com/opentoonz/opentoonz)** — 二维动画制作
`Stars: 6.8k` `NOASSERTION` `更新: 2026-05-26`

🏢 OpenToonz · 动画制作入口；不是 AI 自动化工具

**13.** **[zhouxiaoka/autoclip](https://github.com/zhouxiaoka/autoclip)** — AI 高光提取与自动剪辑
`Stars: 5.5k` `MIT` `更新: 2026-05-08`

🏢 Kris K · AI 智能高光提取与二创剪辑工具；部署较重

**14.** **[browser-use/video-use](https://github.com/browser-use/video-use)** — AI Agent 视频剪辑工具
`Stars: 8.5k` `MIT` `更新: 2026-05-15`

🏢 Browser Use · 用 AI 编程代理剪辑视频；方向新，成熟度需实测

**15.** **[HKUDS/ViMax](https://github.com/HKUDS/ViMax)** — Agent 驱动一站式视频生成
`Stars: 7.7k` `MIT` `更新: 2026-05-26`

🏢 港大数据智能实验室 · 导演/编剧/制片/生成一体化；落地需二次工程化

**16.** **[facebookresearch/pytorchvideo](https://github.com/facebookresearch/pytorchvideo)** — 视频理解研究库
`Stars: 3.6k` `Apache-2.0` `更新: 2026-05-05`

🏢 Meta · 视频理解研究可用；不是生成工具

**17.** **[PaddlePaddle/PaddleVideo](https://github.com/PaddlePaddle/PaddleVideo)** — 视频理解工具箱
`Stars: 1.7k` `Apache-2.0` `更新: 2025-02-12`

🏢 百度 PaddlePaddle · 中文生态可参考；活跃度一般

**18.** **[XPixelGroup/BasicSR](https://github.com/XPixelGroup/BasicSR)** — 视频图像修复
`Stars: 8.3k` `Apache-2.0` `更新: 2024-07-21`

🏢 XPixelGroup · 修复/超分基础库；维护偏旧

**19.** **[PeterL1n/BackgroundMattingV2](https://github.com/PeterL1n/BackgroundMattingV2)** — 视频背景抠像
`Stars: 7.2k` `MIT` `更新: 2024-06-19`

🏢 Peter Lin · 抠像方向实用；维护偏旧

**20.** **[AliaksandrSiarohin/first-order-model](https://github.com/AliaksandrSiarohin/first-order-model)** — 图像驱动动画
`Stars: 15.0k` `MIT` `更新: 2024-11-14`

🏢 Aliaksandr Siarohin · 经典研究项目；新项目需评估替代方案

**21.** **[chatfire-AI/huobao-drama](https://github.com/chatfire-AI/huobao-drama)** — AI 一站式短剧生成平台
`Stars: 12.5k` `未声明` `更新: 2026-05-21`

🏢 AI 火宝 · 一句话生成完整短剧；许可证不清

**22.** **[alecm20/story-flicks](https://github.com/alecm20/story-flicks)** — 故事视频生成
`Stars: 2.4k` `未声明` `更新: 2025-03-12`

🏢 alecm20 · 场景可参考；许可证不清

**23.** **[yuanzhongqiao/deep-comedy-pro](https://github.com/yuanzhongqiao/deep-comedy-pro)** — AI 短剧工厂
`Stars: 4` `未声明` `更新: 2026-05-10`

🏢 yuanzhongqiao · 早期项目；需验证质量

**24.** **[happyhorseai/happyhorse](https://github.com/happyhorseai/happyhorse)** — 文本/图片转 1080p 电影视频
`Stars: 132` `未声明` `更新: 2026-04-08`

🏢 HappyHorse AI · 文本或图片生成电影级视频；成熟度和授权不清

**25.** **[ltaoo/wx_channels_download](https://github.com/ltaoo/wx_channels_download)** — 视频号下载器
`Stars: 6.2k` `NOASSERTION` `更新: 2026-05-24`

🏢 ltaoo · 视频号素材入口；平台规则风险

**26.** **[jianshuo/claude-skills](https://github.com/jianshuo/claude-skills)** — 视频制作 Claude 技能集
`Stars: 62` `MIT；API 可能收费` `更新: 2026-05-26`

🏢 建硕 · 转录/翻译/配音/多机位/字幕/重构等视频技能集

**27.** **[TencentARC/VQFR](https://github.com/TencentARC/VQFR)** — 人脸视频修复
`Stars: 354` `NOASSERTION` `更新: 2022-12-15`

🏢 腾讯 ARC Lab · 可作修复参考；维护较旧


## 四、自媒体

**1.** **[yt-dlp/yt-dlp](https://github.com/yt-dlp/yt-dlp)** — 强力媒体下载器
`Stars: 165.9k` `Unlicense` `更新: 2026-05-25`

🏢 yt-dlp · 素材采集首选；需遵守平台条款

**2.** **[firecrawl/firecrawl](https://github.com/firecrawl/firecrawl)** — AI 网页抓取与结构化
`Stars: 124.9k` `AGPL-3.0` `更新: 2026-05-26`

🏢 Firecrawl · 面向 AI Agent 的网页搜索、抓取和清洗；AGPL 和服务成本需注意

**3.** **[D4Vinci/Scrapling](https://github.com/D4Vinci/Scrapling)** — 自适应网页抓取框架
`Stars: 54.4k` `BSD-3-Clause` `更新: 2026-05-18`

🏢 Karim Shoair · 自适应抓取框架，从单请求到全站爬取；许可清晰

**4.** **[browser-use/browser-use](https://github.com/browser-use/browser-use)** — 浏览器自动化代理
`Stars: 95.7k` `MIT` `更新: 2026-05-26`

🏢 Browser Use · 可处理复杂网页流程；账号风控要重视

**5.** **[langchain-ai/langchain](https://github.com/langchain-ai/langchain)** — 智能体开发平台
`Stars: 137.7k` `MIT` `更新: 2026-05-26`

🏢 LangChain · 内容生成和工具编排生态强；框架复杂度高

**6.** **[soimort/you-get](https://github.com/soimort/you-get)** — 网页媒体下载
`Stars: 56.9k` `NOASSERTION` `更新: 2026-04-30`

🏢 Mort Yao · 素材下载常用；授权需核实

**7.** **[iawia002/lux](https://github.com/iawia002/lux)** — 快速视频下载
`Stars: 31.4k` `MIT` `更新: 2026-03-29`

🏢 Xinzhao Xu · 简洁备选

**8.** **[Panniantong/Agent-Reach](https://github.com/Panniantong/Agent-Reach)** — 全网内容搜索阅读代理
`Stars: 20.3k` `MIT` `更新: 2026-05-18`

🏢 Pnant · Twitter/Reddit/YouTube/B站/小红书全网搜索阅读；零 API 费用

**9.** **[yikart/AiToEarn](https://github.com/yikart/AiToEarn)** — AI 赚钱导航
`Stars: 16.7k` `MIT` `更新: 2026-05-21`

🏢 yikart · 适合找项目线索；不是生产框架

**10.** **[joeseesun/qiaomu-anything-to-notebooklm](https://github.com/joeseesun/qiaomu-anything-to-notebooklm)** — 资料转 NotebookLM
`Stars: 4.7k` `MIT` `更新: 2026-04-28`

🏢 向阳乔木 · 内容整理实用；依赖 NotebookLM 工作流

**11.** **[mvanhorn/last30days-skill](https://github.com/mvanhorn/last30days-skill)** — 跨平台话题深度研究技能
`Stars: 26.6k` `MIT` `更新: 2026-05-22`

🏢 Matt Van Horn · 跨 Reddit/X/YouTube/HN/Polymarket 综合研究；API 成本另算

**12.** **[KKKKhazix/khazix-skills](https://github.com/KKKKhazix/khazix-skills)** — 内容技能合集
`Stars: 11.9k` `MIT；API 可能收费` `更新: 2026-05-08`

🏢 Khazix · 内容流程可参考；需筛选质量

**13.** **[op7418/Humanizer-zh](https://github.com/op7418/Humanizer-zh)** — 中文 AI 降痕
`Stars: 8.4k` `MIT` `更新: 2026-01-19`

🏢 歸藏 · 文案处理可参考；效果需实测

**14.** **[huangserva/skill-prompt-generator](https://github.com/huangserva/skill-prompt-generator)** — AI 人像 Prompt 生成系统
`Stars: 1.4k` `未声明` `更新: 2026-05-10`

🏢 huangserva · 从特征库智能组合生成人像描述 Prompt；许可证不清

**15.** **[CheeMao/ai-content](https://github.com/CheeMao/ai-content)** — AI 内容采集创作发布系统
`Stars: 247` `NOASSERTION` `更新: 2026-03-20`

🏢 CheeMao · 采集、选题、创作、小红书卡图、发布全流程；许可证不清

**16.** **[jackwener/xiaohongshu-cli](https://github.com/jackwener/xiaohongshu-cli)** — 小红书命令行
`Stars: 2.0k` `未声明` `更新: 2026-03-21`

🏢 jakevin · 小红书场景明确；账号和平台风控高

**17.** **[hekaixin66-sketch/xiaohongshuritter](https://github.com/hekaixin66-sketch/xiaohongshuritter)** — 小红书多账号并发 MCP
`Stars: 134` `未声明` `更新: 2026-04-05`

🏢 hekaixin66 · 多账号多并发 MCP 服务；授权和平台规则风险


## 五、金融

**1.** **[OpenBB-finance/OpenBB](https://github.com/OpenBB-finance/OpenBB)** — 金融数据平台
`Stars: 68.1k` `NOASSERTION` `更新: 2026-05-26`

🏢 OpenBB · 投研数据入口强；数据源可能收费

**2.** **[microsoft/qlib](https://github.com/microsoft/qlib)** — AI 量化平台
`Stars: 43.5k` `MIT` `更新: 2026-04-22`

🏢 微软 · AI 量化研究首选之一

**3.** **[vnpy/vnpy](https://github.com/vnpy/vnpy)** — 量化交易框架
`Stars: 41.0k` `MIT` `更新: 2026-05-17`

🏢 vn.py · 中文量化生态成熟；实盘接入需严格风控

**4.** **[mementum/backtrader](https://github.com/mementum/backtrader)** — 策略回测框架
`Stars: 21.7k` `GPL-3.0` `更新: 2024-08-19`

🏢 backtrader · 回测经典；维护偏旧、GPL 约束

**5.** **[freqtrade/freqtrade](https://github.com/freqtrade/freqtrade)** — 加密交易机器人
`Stars: 50.8k` `GPL-3.0` `更新: 2026-05-26`

🏢 freqtrade · 加密策略验证成熟；实盘风险高

**6.** **[TauricResearch/TradingAgents](https://github.com/TauricResearch/TradingAgents)** — 多智能体交易
`Stars: 79.9k` `Apache-2.0` `更新: 2026-05-17`

🏢 Tauric Research · Agent 投研代表项目；先做研究别直接实盘

**7.** **[Open-Dev-Society/OpenStock](https://github.com/Open-Dev-Society/OpenStock)** — 开源行情追踪与分析平台
`Stars: 12.2k` `AGPL-3.0` `更新: 2026-05-02`

🏢 Open Dev Society · 开源行情追踪、个性化提醒、公司深度分析；AGPL 和部署成本

**8.** **[ZhuLinsen/daily_stock_analysis](https://github.com/ZhuLinsen/daily_stock_analysis)** — LLM 驱动 A/H/美股智能分析
`Stars: 39.0k` `MIT` `更新: 2026-05-26`

🏢 ZhuLinsen · 多数据源行情 + 实时新闻 + LLM 决策仪表盘 + 多渠道推送

**9.** **[HKUDS/Vibe-Trading](https://github.com/HKUDS/Vibe-Trading)** — 个人交易 Agent
`Stars: 8.8k` `MIT` `更新: 2026-05-25`

🏢 港大数据智能实验室 · 个人交易 Agent 方向活跃；需严谨回测

**10.** **[polakowo/vectorbt](https://github.com/polakowo/vectorbt)** — 高性能向量化回测引擎
`Stars: 7.7k` `NOASSERTION` `更新: 2026-04-25`

🏢 Oleg Polakow · 千级策略并行回测；授权需核实

**11.** **[pmorissette/bt](https://github.com/pmorissette/bt)** — 组合回测工具
`Stars: 2.9k` `MIT` `更新: 2026-05-05`

🏢 Philippe Morissette · 组合回测轻量；生态不如主流平台

**12.** **[TA-Lib/ta-lib-python](https://github.com/TA-Lib/ta-lib-python)** — 技术指标库
`Stars: 12.0k` `BSD-2-Clause` `更新: 2026-03-16`

🏢 TA-Lib · 指标计算基础库；不是完整平台

**13.** **[quantopian/zipline](https://github.com/quantopian/zipline)** — 量化回测库
`Stars: 19.8k` `Apache-2.0` `更新: 2024-02-13`

🏢 Quantopian · 经典回测框架；更新偏旧

**14.** **[binance/binance-connector-python](https://github.com/binance/binance-connector-python)** — 币安 API 连接器
`Stars: 2.9k` `MIT` `更新: 2026-05-22`

🏢 Binance 币安 · 交易所接口清晰；交易所和地区合规风险

**15.** **[okx/agent-trade-kit](https://github.com/okx/agent-trade-kit)** — OKX 交易 MCP 服务器
`Stars: 313` `MIT` `更新: 2026-05-20`

🏢 OKX · 通过 MCP 连接 AI Agent 到现货/合约/期权/网格；实盘风险高

**16.** **[Fincept-Corporation/FinceptTerminal](https://github.com/Fincept-Corporation/FinceptTerminal)** — 交互式金融数据分析终端
`Stars: 24.2k` `NOASSERTION` `更新: 2026-05-26`

🏢 Fincept · 市场分析、投研和经济数据的交互式终端；许可证不清

**17.** **[brokermr810/QuantDinger](https://github.com/brokermr810/QuantDinger)** — 多市场 AI 量化交易平台
`Stars: 6.6k` `Apache-2.0` `更新: 2026-05-25`

🏢 QuantDinger · 覆盖加密、股票、外汇的回测与实盘；成熟度需实测

**18.** **[anthropics/financial-services](https://github.com/anthropics/financial-services)** — 金融 AI 示例
`Stars: 27.9k` `Apache-2.0` `更新: 2026-05-21`

🏢 Anthropic · 示例参考价值高；不是完整产品

**19.** **[virattt/dexter](https://github.com/virattt/dexter)** — 金融深度研究 Agent
`Stars: 26.5k` `未声明` `更新: 2026-05-24`

🏢 Virat Singh · 自主执行深度金融研究的 Agent；许可证不清

**20.** **[koala73/worldmonitor](https://github.com/koala73/worldmonitor)** — AI 实时全球情报监控面板
`Stars: 55.0k` `NOASSERTION` `更新: 2026-05-26`

🏢 Elie Habib · AI 驱动新闻聚合、地缘政治和基础设施监控；许可证不清


## 六、设计

**1.** **[shadcn-ui/ui](https://github.com/shadcn-ui/ui)** — 可复制粘贴的 UI 组件集
`Stars: 115.1k` `MIT` `更新: 2026-05-25`

🏢 shadcn · 现代前端组件首选之一

**2.** **[ant-design/ant-design](https://github.com/ant-design/ant-design)** — 企业 React 组件
`Stars: 98.1k` `MIT` `更新: 2026-05-26`

🏢 蚂蚁集团 · 企业后台成熟度高

**3.** **[mui/material-ui](https://github.com/mui/material-ui)** — Material 组件库
`Stars: 98.4k` `MIT` `更新: 2026-05-25`

🏢 MUI · 国际化生态强

**4.** **[tailwindlabs/tailwindcss](https://github.com/tailwindlabs/tailwindcss)** — 原子化 CSS 框架
`Stars: 95.1k` `MIT` `更新: 2026-05-24`

🏢 Tailwind Labs · 快速搭建 UI 体系

**5.** **[storybookjs/storybook](https://github.com/storybookjs/storybook)** — 组件开发测试文档工具
`Stars: 90.1k` `MIT` `更新: 2026-05-26`

🏢 Storybook · 组件工程化和设计系统必备

**6.** **[penpot/penpot](https://github.com/penpot/penpot)** — 开源协作设计工具
`Stars: 48.5k` `MPL-2.0` `更新: 2026-05-26`

🏢 Penpot · 开源 Figma 替代方向

**7.** **[nexu-io/open-design](https://github.com/nexu-io/open-design)** — 开源 AI 设计工具
`Stars: 53.1k` `Apache-2.0；API 可能收费` `更新: 2026-05-26`

🏢 nexu · 本地优先的开源 Claude Design 替代方案，71 套设计系统

**8.** **[plasmicapp/plasmic](https://github.com/plasmicapp/plasmic)** — 可视化 React 构建
`Stars: 6.8k` `MIT` `更新: 2026-05-25`

🏢 Plasmic · 可视化构建能力强；平台绑定需评估

**9.** **[webstudio-is/webstudio](https://github.com/webstudio-is/webstudio)** — 开源网站构建器
`Stars: 8.6k` `AGPL-3.0` `更新: 2026-05-26`

🏢 Webstudio · 网站构建器方向；AGPL 约束

**10.** **[BuilderIO/gpt-crawler](https://github.com/BuilderIO/gpt-crawler)** — 站点知识抓取
`Stars: 22.2k` `ISC` `更新: 2025-07-07`

🏢 Builder.io · 可为设计/站点重构准备上下文

**11.** **[figma/plugin-samples](https://github.com/figma/plugin-samples)** — Figma 插件示例
`Stars: 1.8k` `MIT` `更新: 2026-03-23`

🏢 Figma · 插件开发参考

**12.** **[VoltAgent/awesome-design-md](https://github.com/VoltAgent/awesome-design-md)** — 品牌设计系统 DESIGN.md 合集
`Stars: 84.6k` `MIT` `更新: 2026-05-18`

🏢 VoltAgent · 品牌设计系统 DESIGN.md 文件集合；不是工具

**13.** **[JCodesMore/ai-website-cloner-template](https://github.com/JCodesMore/ai-website-cloner-template)** — AI 网站克隆模板
`Stars: 15.5k` `MIT；API 可能收费` `更新: 2026-05-07`

🏢 JCodesMore · 站点克隆工作流可参考；依赖 SaaS/API

**14.** **[nextlevelbuilder/ui-ux-pro-max-skill](https://github.com/nextlevelbuilder/ui-ux-pro-max-skill)** — UIUX 提示技能
`Stars: 83.2k` `MIT` `更新: 2026-04-03`

🏢 Next Level Builder · UI 提示流程可参考


## 七、编程 & Agent

**1.** **[openai/codex](https://github.com/openai/codex)** — 终端编程 Agent
`Stars: 86.1k` `开源；模型另付` `更新: 未在原文记录`

🏢 OpenAI · 编程 Agent 工作流核心入口

**2.** **[All-Hands-AI/OpenHands](https://github.com/All-Hands-AI/OpenHands)** — 软件工程 Agent 平台
`Stars: 75.0k` `开源；模型另付` `更新: 未在原文记录`

🏢 All Hands AI · 软件工程 Agent 平台成熟度高

**3.** **[bytedance/deer-flow](https://github.com/bytedance/deer-flow)** — 长任务超级 Agent
`Stars: 69.7k` `MIT；模型另付` `更新: 2026-05-26`

🏢 字节跳动 · 长任务、子代理、记忆、沙箱架构完整

**4.** **[openclaw/openclaw](https://github.com/openclaw/openclaw)** — 跨平台个人 AI 助理
`Stars: 374.9k` `MIT；模型另付` `更新: 2026-05-26`

🏢 OpenClaw · 个人数据自托管和多通道集成好

**5.** **[microsoft/autogen](https://github.com/microsoft/autogen)** — Agent AI 编程框架
`Stars: 58.4k` `开源；模型另付` `更新: 未在原文记录`

🏢 微软 · 多 Agent 编排生态强

**6.** **[langchain-ai/langgraph](https://github.com/langchain-ai/langgraph)** — 弹性 Agent 构建框架
`Stars: 33.1k` `开源；模型另付` `更新: 未在原文记录`

🏢 LangChain · 可控 Agent 流程编排强

**7.** **[crewAIInc/crewAI](https://github.com/crewAIInc/crewAI)** — 角色协作 Agent 框架
`Stars: 52.3k` `开源；模型另付` `更新: 未在原文记录`

🏢 crewAI · 角色协作上手快；复杂任务需验证

**8.** **[nousresearch/hermes-agent](https://github.com/nousresearch/hermes-agent)** — 自成长个人 Agent
`Stars: 169.1k` `MIT；模型/API 另付` `更新: 2026-05-25`

🏢 Nous Research · 技能学习和个人助理形态完整

**9.** **[affaan-m/ECC](https://github.com/affaan-m/ECC)** — Agent 性能优化系统
`Stars: 194.8k` `MIT；模型另付` `更新: 2026-05-25`

🏢 Affaan Mustafa · 覆盖技能、本能、记忆、安全的 Agent 性能优化

**10.** **[obra/superpowers](https://github.com/obra/superpowers)** — Agent 技能方法论
`Stars: 208.3k` `MIT` `更新: 2026-05-04`

🏢 Jesse Vincent · 跨 Claude、Codex、OpenCode 的流程资产

**11.** **[addyosmani/agent-skills](https://github.com/addyosmani/agent-skills)** — 工程技能集合
`Stars: 46.2k` `MIT` `更新: 2026-05-24`

🏢 Addy Osmani (Google) · 工程质量门槛和流程成熟

**12.** **[anthropics/skills](https://github.com/anthropics/skills)** — Claude 官方技能集
`Stars: 141.4k` `未声明许可证` `更新: 2026-05-19`

🏢 Anthropic · 标准参考价值高；商用复用需谨慎

**13.** **[MiniMax-AI/skills](https://github.com/MiniMax-AI/skills)** — MiniMax 技能集合
`Stars: 12.1k` `有 LICENSE` `更新: 2026-04-18`

🏢 MiniMax · 国产模型技能参考

**14.** **[vercel-labs/skills](https://github.com/vercel-labs/skills)** — Vercel 技能集合
`Stars: 20.2k` `免费；需核实` `更新: 2026-05-23`

🏢 Vercel · 技能发现和模板参考

**15.** **[HKUDS/OpenSpace](https://github.com/HKUDS/OpenSpace)** — Agent 自进化开放平台
`Stars: 6.4k` `MIT；API 另付` `更新: 2026-05-21`

🏢 港大数据智能实验室 · 让 Agent 更智能、低成本、自进化的开放平台

**16.** **[HKUDS/CLI-Anything](https://github.com/HKUDS/CLI-Anything)** — 软件 Agent 化 CLI 框架
`Stars: 40.7k` `Apache-2.0` `更新: 2026-05-23`

🏢 港大数据智能实验室 · 让所有软件变为 Agent 可操作的 CLI

**17.** **[paperclipai/paperclip](https://github.com/paperclipai/paperclip)** — 开源 Agent 管理应用
`Stars: 67.8k` `MIT；模型另付` `更新: 2026-05-25`

🏢 Paperclip · 团队 Agent 管理与协作应用

**18.** **[thunlp/ProactiveAgent](https://github.com/thunlp/ProactiveAgent)** — 主动事件 Agent
`Stars: 604` `Apache-2.0；API 另付` `更新: 2026-05-12`

🏢 清华 NLP · 主动 Agent 学术参考

**19.** **[davila7/claude-code-templates](https://github.com/davila7/claude-code-templates)** — Claude 配置模板 CLI
`Stars: 27.6k` `MIT；云服务另付` `更新: 2026-05-26`

🏢 Daniel Avila · 模板和监控一体；SaaS 依赖多

**20.** **[hesamsheikh/octogent](https://github.com/hesamsheikh/octogent)** — 多代理编程看板
`Stars: 1.1k` `MIT；模型另付` `更新: 2026-04-20`

🏢 Hesam Sheikh · 多 Claude/Codex 会话管理

**21.** **[ruvnet/ruflo](https://github.com/ruvnet/ruflo)** — Claude 多 Agent 编排平台
`Stars: 55.5k` `MIT` `更新: 2026-05-26`

🏢 rUv · 多 Agent 集群编排、自学习、RAG 集成

**22.** **[code-yeongyu/oh-my-openagent](https://github.com/code-yeongyu/oh-my-openagent)** — 全能 Agent Harness
`Stars: 59.7k` `Sustainable Use License` `更新: 2026-05-26`

🏢 YeonGyu Kim · 面向多 Harness；许可证限制更强

**23.** **[EveryInc/compound-engineering-plugin](https://github.com/EveryInc/compound-engineering-plugin)** — 复合工程插件
`Stars: 17.3k` `MIT` `更新: 2026-05-24`

🏢 Every · 工程流程插件化

**24.** **[farion1231/cc-switch](https://github.com/farion1231/cc-switch)** — 跨平台 AI 助手桌面端
`Stars: 82.0k` `MIT` `更新: 2026-05-26`

🏢 Jason Young · Claude Code/Codex/Gemini CLI 等多工具统一桌面助手

**25.** **[kepano/obsidian-skills](https://github.com/kepano/obsidian-skills)** — Obsidian Agent 技能
`Stars: 33.2k` `MIT` `更新: 2026-05-24`

🏢 Steph Ango (Obsidian CEO) · 知识库自动化好

**26.** **[K-Dense-AI/claude-scientific-skills](https://github.com/K-Dense-AI/claude-scientific-skills)** — 科研 Agent 技能
`Stars: 26.1k` `MIT；抓取服务可能另付` `更新: 2026-05-25`

🏢 K-Dense · 科研场景专业

**27.** **[mattpocock/skills](https://github.com/mattpocock/skills)** — 工程师常用技能
`Stars: 107.2k` `MIT` `更新: 2026-05-20`

🏢 Matt Pocock · TypeScript 工程经验强

**28.** **[ant-design/antd-skill](https://github.com/ant-design/antd-skill)** — Ant Design 技能
`Stars: 84` `MIT` `更新: 2026-03-27`

🏢 蚂蚁集团 · 前端设计规范技能

**29.** **[antvis/chart-visualization-skills](https://github.com/antvis/chart-visualization-skills)** — 图表可视化技能
`Stars: 299` `MIT` `更新: 2026-05-25`

🏢 蚂蚁 AntV · 数据可视化 Agent 技能

**30.** **[coreyhaines31/marketingskills](https://github.com/coreyhaines31/marketingskills)** — 营销 Agent 技能
`Stars: 30.7k` `MIT` `更新: 2026-05-21`

🏢 Corey Haines · 垂直营销流程清晰

**31.** **[tinyhumansai/openhuman](https://github.com/tinyhumansai/openhuman)** — 开源个人 AI 超级智能
`Stars: 28.5k` `GPL-3.0` `更新: 2026-05-26`

🏢 Tiny Humans · 私有、简洁、强大的个人 AI；GPL 约束

**32.** **[karpathy/autoresearch](https://github.com/karpathy/autoresearch)** — 单 GPU 自动化模型训练研究
`Stars: 83.6k` `未声明许可证；算力另付` `更新: 2026-03-25`

🏢 Andrej Karpathy · 单 GPU nanochat 自动训练实验；授权和稳定性不足

**33.** **[AndyMik90/Aperant](https://github.com/AndyMik90/Aperant)** — 多代理编码框架
`Stars: 14.3k` `AGPL-3.0` `更新: 2026-03-23`

🏢 André Mikalsen · 计划-构建-验证闭环；AGPL 约束

**34.** **[iamzhihuix/skills-manage](https://github.com/iamzhihuix/skills-manage)** — Skills 桌面管理器
`Stars: 1.9k` `Apache-2.0` `更新: 2026-05-02`

🏢 iamzhihuix · 技能管理层；不是执行框架

**35.** **[nicedreamzapp/claude-code-local](https://github.com/nicedreamzapp/claude-code-local)** — 本地模型跑 Claude
`Stars: 2.7k` `MIT` `更新: 2026-05-22`

🏢 Nice Dreamz · 本地隐私方向；依赖硬件/模型

**36.** **[multica-ai/andrej-karpathy-skills](https://github.com/multica-ai/andrej-karpathy-skills)** — Karpathy 编码准则
`Stars: 157.5k` `未声明许可证` `更新: 2026-04-20`

🏢 multica-ai · 单文件易复制；授权需谨慎

**37.** **[Donchitos/Claude-Code-Game-Studios](https://github.com/Donchitos/Claude-Code-Game-Studios)** — Claude 游戏开发工作室
`Stars: 20.1k` `MIT` `更新: 2026-05-13`

🏢 Donchitos · 游戏开发流程模板

**38.** **[msitarzewski/agency-agents](https://github.com/msitarzewski/agency-agents)** — AI 专家角色库
`Stars: 105.4k` `MIT` `更新: 2026-04-11`

🏢 Michael Sitarzewski · 角色覆盖广；不是可运行框架

**39.** **[jnMetaCode/agency-agents-zh](https://github.com/jnMetaCode/agency-agents-zh)** — 中文专家角色库
`Stars: 13.0k` `MIT` `更新: 2026-05-19`

🏢 AI不止语 · 中文本地化好；依赖上游内容


## 八、浏览器 / 桌面自动化 / 工具底座

**1.** **[simular-ai/agent-s](https://github.com/simular-ai/agent-s)** — 像人一样操作电脑的 Agent
`Stars: 11.6k` `Apache-2.0；API 另付` `更新: 2026-05-13`

🏢 Simular AI · 桌面 CUA 首选验证项

**2.** **[TurixAI/TuriX-CUA](https://github.com/TurixAI/TuriX-CUA)** — 桌面动作模型
`Stars: 3.0k` `MIT` `更新: 2026-05-25`

🏢 TuriX AI · 桌面动作执行明确

**3.** **[browser-use/browser-harness](https://github.com/browser-use/browser-harness)** — 自修复浏览器 Agent Harness
`Stars: 13.8k` `MIT` `更新: 2026-05-20`

🏢 Browser Use · 自修复机制让 LLM 完成复杂浏览器任务

**4.** **[vercel-labs/agent-browser](https://github.com/vercel-labs/agent-browser)** — AI Agent 浏览器自动化 CLI
`Stars: 34.4k` `Apache-2.0` `更新: 2026-05-20`

🏢 Vercel · 快速浏览器自动化

**5.** **[openclaw/Peekaboo](https://github.com/openclaw/Peekaboo)** — macOS 截屏与视觉问答工具
`Stars: 4.5k` `MIT` `更新: 2026-05-25`

🏢 OpenClaw · macOS 截屏 + 可选 VQA 的 MCP 服务

**6.** **[microsoft/playwright](https://github.com/microsoft/playwright)** — 浏览器自动化基础库
`Stars: 89.6k` `Apache-2.0` `更新: 未在原文记录`

🏢 微软 · Web 自动化标准工具

**7.** **[puppeteer/puppeteer](https://github.com/puppeteer/puppeteer)** — Chrome/Firefox 自动化库
`Stars: 94.4k` `Apache-2.0` `更新: 未在原文记录`

🏢 Google · Chrome 自动化成熟

**8.** **[SeleniumHQ/selenium](https://github.com/SeleniumHQ/selenium)** — WebDriver 生态
`Stars: 34.1k` `Apache-2.0` `更新: 未在原文记录`

🏢 Selenium · 企业兼容性强

**9.** **[modelcontextprotocol/servers](https://github.com/modelcontextprotocol/servers)** — MCP 工具服务器集合
`Stars: 86.3k` `开源；需核实` `更新: 未在原文记录`

🏢 Anthropic MCP · Agent 工具扩展入口

**10.** **[public-apis/public-apis](https://github.com/public-apis/public-apis)** — 免费 API 目录
`Stars: 437.3k` `MIT` `更新: 2026-05-26`

🏢 public-apis · 可给 Agent 扩工具源

**11.** **[googleworkspace/cli](https://github.com/googleworkspace/cli)** — Google Workspace CLI
`Stars: 26.6k` `Apache-2.0；Google API 账号` `更新: 2026-03-31`

🏢 Google · 办公套件可被 Agent 调用

**12.** **[Tencent/openclaw-weixin](https://github.com/Tencent/openclaw-weixin)** — OpenClaw 微信插件
`Stars: 526` `MIT 文本` `更新: 2026-05-18`

🏢 腾讯 · 微信通道价值高；登录和合规约束

**13.** **[clawvader-tech/hermes-telegram-miniapp](https://github.com/clawvader-tech/hermes-telegram-miniapp)** — Telegram Mini App 前端
`Stars: 226` `MIT` `更新: 2026-04-15`

🏢 clawvader · Telegram Mini App v2.0 的 10 页移动端 UI；需配后端

**14.** **[antirez/ds4](https://github.com/antirez/ds4)** — DeepSeek 4 本地推理引擎
`Stars: 12.0k` `MIT` `更新: 2026-05-26`

🏢 antirez (Redis 作者) · DeepSeek 4 Flash 的 Metal/CUDA 本地推理

**15.** **[Mininglamp-AI/cider](https://github.com/Mininglamp-AI/cider)** — Apple Silicon INT8 推理加速
`Stars: 308` `MIT` `更新: 2026-05-11`

🏢 明略科技 · M5 芯片 INT8 TensorOps 加速 LLM 推理 1.2-1.9 倍

**16.** **[AndrewNgGirl/SkillLens](https://github.com/AndrewNgGirl/SkillLens)** — Agent Skill 评估打分工具
`Stars: 59` `MIT` `更新: 2026-05-17`

🏢 AndrewNg 小迷妹 · 适合筛选技能库；成熟度需验证

**17.** **[kangarooking/cangjie-skill](https://github.com/kangarooking/cangjie-skill)** — 书籍蒸馏为 Agent 技能
`Stars: 979` `MIT` `更新: 2026-05-04`

🏢 kangarooking · 内容型技能可复用；非工程框架

**18.** **[FujiwaraChoki/MoneyPrinterV2](https://github.com/FujiwaraChoki/MoneyPrinterV2)** — AI 自动化在线赚钱工具
`Stars: 30.6k` `AGPL-3.0；平台/API 可能另付` `更新: 2026-05-15`

🏢 FujiwaraChoki · 自动化在线赚钱流程；AGPL 与平台风控风险


## 九、官网 / 产品页 / 非单仓库入口

这些链接不是可直接评估的单一 GitHub 仓库，建议只作为产品或组织入口，再按具体仓库、价格、许可和数据合规单独确认。

**1.** **[Marvis](https://marvis.qq.com/)** — 腾讯系统级助手
`官网 2026-05 可下载`

闭源，本地/云端模型和桌面权限需确认

**2.** **[CodeBuddy WorkBuddy](https://www.codebuddy.cn/work/)** — 腾讯办公 Agent
`定价页 2026-05-15 后生效`

商业产品，个人专业版 58 元/月，企业版 198/316 元/月起

**3.** **[QoderWake](https://qoder.com/qoderwake)** — 24 小时数字员工
`官网可访问；未见仓库`

闭源云产品，需信任平台

**4.** **[Helio](https://www.helio.im/)** — AI 原生团队工作区
`官网可访问`

闭源，团队协作平台

**5.** **[Clockless AI](https://clockless.ai/)** — 客户关系 AI 门户
`官网可访问`

闭源 SaaS，需销售确认

**6.** **[ClawinLink](https://claw.baolieguoshi.com/)** — Agent 消息网关
`官网内测`

微信/QQ 通道，合规和接入门槛高

**7.** **[ghuntley](https://github.com/ghuntley)** — Agent 方法论作者
`个人主页`

不是单仓库，适合看其教程和代表仓库

**8.** **[TauricResearch](https://github.com/TauricResearch)** — 金融 Agent 组织
`GitHub 组织主页`

应按组织内具体仓库评估

**9.** **[Binance](https://github.com/binance)** — Binance 组织
`GitHub 组织主页`

应按具体 SDK/接口仓库评估

**10.** **[OpenToonz 官网](https://opentoonz.github.io/e/index.html)** — 开源二维动画软件
`官网入口`

GitHub 仓库应看 opentoonz/opentoonz

**11.** **[yikeai](https://www.yikeai.com/#/home)** — 商业 AI 视频平台
`官网入口`

非仓库，价格和素材授权需确认

**12.** **[Wind 金融技能页](https://aifinmarket.wind.com.cn/skill.md)** — Wind 金融技能页
`页面入口`

商业数据/服务属性需确认

**13.** **[MCPMarket UI Prompt Generator](https://mcpmarket.com/zh/tools/skills/ui-prompt-generator)** — UI 提示工具页
`页面入口`

非仓库，无法按开源许可判断

**14.** **[腾讯 ArDot](https://ardot.tencent.com/)** — 腾讯设计平台
`官网入口`

非仓库，商业和平台绑定需确认

## 十、注意事项

**换脸、人脸识别、桌面控制、浏览器控制、微信/QQ 通道**
`涉及隐私、账号、平台规则和误操作风险`

必须做权限隔离、日志审计、人工确认和合规边界

**金融交易 Agent / 交易所 SDK**
`容易被误用为实盘自动交易`

先做研究、回测、模拟盘；实盘需要风控和合规审查

## 联系方式

| 个人微信 | 公众号 |
|:---:|:---:|
| <img src="./wechat.jpg" width="200" /> | <img src="./gzh.png" width="200" /> |
| 扫码添加微信 | 扫码关注公众号 |
