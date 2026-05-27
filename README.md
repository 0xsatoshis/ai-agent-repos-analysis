# GitHub AI / Agent 仓库分类推荐清单

GitHub AI / Agent 仓库分类推荐清单，覆盖图片生成、语音识别、视频自动化、金融研究、Agent 编程、浏览器自动化等方向。

生成时间：2026-05-26（Asia/Shanghai）

数据来源：原始两份分析文档、GitHub REST API、仓库 README/常见依赖文件探测；非 GitHub 链接仅做入口级判断。GitHub 的 `pushed_at` / 最后提交时间以原文档记录为准，日期口径可能包含 UTC 与 CST 差异。

排序口径：
- 每个分类按"推荐优先看"的顺序排列，综合考虑工程可用性、生态成熟度、活跃度、许可证清晰度、落地成本和风险。
- 同类工具中，优先推荐可直接用于生产/研究工作流的仓库；素材集、提示词集、方法论和入口页排在后面。
- "免费/开源"只指仓库代码本身；模型 API、云服务、交易所、数据源、GPU/Apple Silicon、本地存储、平台账号等可能另行收费。

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

| 推荐 | 项目 | 简介 | 最后更新 | 许可/付费 | 外部依赖 | 推荐理由 / 风险 |
|---:|---|---|---:|---|---|---|
| 1 | [Comfy-Org/ComfyUI](https://github.com/Comfy-Org/ComfyUI) | 节点式生成工作流 | 2026-05-26 | GPL-3.0；代码免费开源 | requirements、pyproject；ComfyUI、Node | 本地图片工作流首选，生态强；部署和显存成本较高 |
| 2 | [AUTOMATIC1111/stable-diffusion-webui](https://github.com/AUTOMATIC1111/stable-diffusion-webui) | SD 网页生成界面 | 2026-03-02 | AGPL-3.0 | Python/模型依赖 | 插件和资料最多；AGPL 商业复用要谨慎 |
| 3 | [huggingface/diffusers](https://github.com/huggingface/diffusers) | 扩散模型库 | 2026-05-26 | Apache-2.0 | Python、Torch | 工程化调用模型更合适；需要自己搭 UI/流程 |
| 4 | [facebookresearch/segment-anything](https://github.com/facebookresearch/segment-anything) | 图像分割模型 | 2024-09-18 | Apache-2.0 | Python、Torch | 抠图/分割基础能力强；模型和算力另算 |
| 5 | [lllyasviel/ControlNet](https://github.com/lllyasviel/ControlNet) | 可控图像生成 | 2024-02-25 | Apache-2.0 | Python、Torch | 姿态/边缘/深度控制经典方案；维护节奏偏旧 |
| 6 | [xinntao/Real-ESRGAN](https://github.com/xinntao/Real-ESRGAN) | 图像视频超分 | 2024-08-06 | BSD-3-Clause | Python、Torch | 图片/视频增强实用；更新偏旧但仍常用 |
| 7 | [TencentARC/GFPGAN](https://github.com/TencentARC/GFPGAN) | 人脸修复增强 | 2024-07-26 | NOASSERTION | Python、Torch | 人脸修复效果好；许可证不清需核实 |
| 8 | [serengil/deepface](https://github.com/serengil/deepface) | 人脸识别分析库 | 2026-05-13 | MIT；代码免费开源 | requirements、setup、Dockerfile | 人脸识别/分析成熟；涉及隐私合规 |
| 9 | [facefusion/facefusion](https://github.com/facefusion/facefusion) | 人脸融合工具 | 2026-05-26 | NOASSERTION；仓库免费 | requirements | 活跃、可落地；换脸场景需合规审查 |
| 10 | [lllyasviel/Fooocus](https://github.com/lllyasviel/Fooocus) | 轻量图像生成 | 2025-12-01 | GPL-3.0 | Python/模型依赖 | 上手简单；扩展性不如 ComfyUI |
| 11 | [Stability-AI/generative-models](https://github.com/Stability-AI/generative-models) | 扩散模型代码 | 2025-12-16 | MIT | Python、模型权重 | 适合研究模型本体；落地需工程封装 |
| 12 | [IDEA-Research/GroundingDINO](https://github.com/IDEA-Research/GroundingDINO) | 开放词检测 | 2024-08-12 | Apache-2.0 | Python、Torch | 与 SAM/自动标注组合价值高；部署成本较高 |
| 13 | [antvis/Infographic](https://github.com/antvis/Infographic) | 图表信息可视化 | 2026-05-06 | MIT；代码免费开源 | package.json | 信息图方向实用；偏可视化不是图片生成 |
| 14 | [EvoLinkAI/awesome-gpt-image-2-API-and-Prompts](https://github.com/EvoLinkAI/awesome-gpt-image-2-API-and-Prompts) | 图像 API 提示集 | 2026-05-22 | CC0-1.0 | 有代码依赖 | 提示词积累有价值；依赖具体模型效果 |
| 15 | [freestylefly/awesome-gpt-image-2](https://github.com/freestylefly/awesome-gpt-image-2) | 图像提示资源库 | 2026-05-25 | MIT | package.json | 适合做提示素材库；不是生产工具 |
| 16 | [YouMind-OpenLab/awesome-gpt-image-2](https://github.com/YouMind-OpenLab/awesome-gpt-image-2) | GPT 图像提示集 | 2026-05-26 | NOASSERTION | package.json、OpenAI | 活跃；许可证不清 |
| 17 | [YouMind-OpenLab/awesome-nano-banana-pro-prompts](https://github.com/YouMind-OpenLab/awesome-nano-banana-pro-prompts) | Nano 提示词合集 | 2026-05-26 | NOASSERTION | package.json | 可作素材参考；许可证不清 |
| 18 | [JimLiu/baoyu-skills](https://github.com/JimLiu/baoyu-skills) | 宝玉技能合集 | 2026-05-26 | 未声明 | package.json、Node | 技能资产可参考；复用需确认授权 |

## 二、语音

| 推荐 | 项目 | 简介 | 最后更新 | 许可/付费 | 外部依赖 | 推荐理由 / 风险 |
|---:|---|---|---:|---|---|---|
| 1 | [openai/whisper](https://github.com/openai/whisper) | 通用语音识别 | 2026-04-15 | MIT；代码免费；API 可能收费 | requirements、pyproject、ffmpeg、Torch | ASR 首选基线，生态广 |
| 2 | [ggml-org/whisper.cpp](https://github.com/ggml-org/whisper.cpp) | 本地 Whisper 推理 | 2026-05-26 | MIT | C/C++、模型文件 | 本地低成本部署优秀；功能聚焦推理 |
| 3 | [NVIDIA-NeMo/NeMo](https://github.com/NVIDIA-NeMo/NeMo) | 语音 AI 框架 | 2026-05-26 | Apache-2.0 | Python、GPU | 企业级语音/多模态框架；部署较重 |
| 4 | [espnet/espnet](https://github.com/espnet/espnet) | 端到端语音套件 | 2026-05-25 | Apache-2.0 | Python、深度学习依赖 | 研究和训练能力强；上手成本高 |
| 5 | [OpenBMB/VoxCPM](https://github.com/OpenBMB/VoxCPM) | 中文语音生成模型 | 2026-05-22 | Apache-2.0 | pyproject、OpenAI 关键词 | 中文方向值得优先验证；模型资源另算 |
| 6 | [rhasspy/piper](https://github.com/rhasspy/piper) | 本地 TTS 系统 | 2025-08-26 | MIT | ONNX/本地模型 | 本地 TTS 轻量实用；音色质量需实测 |
| 7 | [suno-ai/bark](https://github.com/suno-ai/bark) | 生成式语音模型 | 2024-08-19 | MIT | Python、模型权重 | 生成能力强；维护偏旧 |
| 8 | [coqui-ai/TTS](https://github.com/coqui-ai/TTS) | 开源 TTS 工具箱 | 2024-08-16 | MPL-2.0 | requirements、pyproject、Dockerfile | 星标高、功能全；维护偏旧 |
| 9 | [snakers4/silero-models](https://github.com/snakers4/silero-models) | 轻量语音模型 | 2026-05-20 | NOASSERTION | Python/模型 | 轻量模型适合边缘验证；授权需核实 |
| 10 | [microsoft/SpeechT5](https://github.com/microsoft/SpeechT5) | 语音文本预训练 | 2024-04-24 | MIT | Python、模型 | 研究参考价值高；更新偏旧 |
| 11 | [abus-aikorea/voice-pro](https://github.com/abus-aikorea/voice-pro) | 语音处理工作台 | 2025-12-05 | GPL-3.0 | 有代码依赖 | 工具形态完整；需实测稳定性 |
| 12 | [mozilla/DeepSpeech](https://github.com/mozilla/DeepSpeech) | 离线语音识别 | 2025-06-19 | MPL-2.0 | Python/模型 | 历史项目参考；新项目优先 Whisper 系 |

## 三、视频

| 推荐 | 项目 | 简介 | 最后更新 | 许可/付费 | 外部依赖 | 推荐理由 / 风险 |
|---:|---|---|---:|---|---|---|
| 1 | [FFmpeg/FFmpeg](https://github.com/FFmpeg/FFmpeg) | 音视频处理核心 | 2026-05-26 | NOASSERTION | C/C++ | 所有视频自动化底座；许可证细节需按组件核实 |
| 2 | [remotion-dev/remotion](https://github.com/remotion-dev/remotion) | React 生成视频 | 2026-05-26 | NOASSERTION | Node、React | 工程化视频渲染强；商业授权需核实 |
| 3 | [heygen-com/hyperframes](https://github.com/heygen-com/hyperframes) | HTML 视频生成框架 | 2026-05-26 | Apache-2.0 | package.json、Node、OpenAI | 适合代码化视频、字幕、动画 |
| 4 | [harry0703/MoneyPrinterTurbo](https://github.com/harry0703/MoneyPrinterTurbo) | 一键短视频生成 | 2026-05-26 | MIT | requirements、pyproject、Dockerfile、OpenAI | 短视频自动化最值得先看；API/素材/平台成本另算 |
| 5 | [Zulko/moviepy](https://github.com/Zulko/moviepy) | Python 视频剪辑 | 2026-03-07 | MIT | Python、FFmpeg | Python 自动剪辑实用；复杂渲染不如 Remotion |
| 6 | [mifi/lossless-cut](https://github.com/mifi/lossless-cut) | 无损视频剪切 | 2026-05-23 | GPL-2.0 | Electron、FFmpeg | 素材切割非常实用；不是生成框架 |
| 7 | [obsproject/obs-studio](https://github.com/obsproject/obs-studio) | 直播录屏软件 | 2026-05-23 | GPL-2.0 | C++/桌面依赖 | 录制/直播基础能力强；二开成本高 |
| 8 | [hacksider/Deep-Live-Cam](https://github.com/hacksider/Deep-Live-Cam) | 实时换脸工具 | 2026-05-24 | AGPL-3.0 | requirements | 社区强、活跃；换脸合规和 AGPL 风险高 |
| 9 | [AIDC-AI/Pixelle-Video](https://github.com/AIDC-AI/Pixelle-Video) | 视频生成模型 | 2026-05-18 | Apache-2.0 | pyproject、Dockerfile、ComfyUI | 视频生成方向活跃；部署成本高 |
| 10 | [MemeCalculate/moyin-creator](https://github.com/MemeCalculate/moyin-creator) | 模板视频创作 | 2026-05-25 | AGPL-3.0 | package.json、Node、React | 模板化创作可用；AGPL 商用限制 |
| 11 | [elebumm/RedditVideoMakerBot](https://github.com/elebumm/RedditVideoMakerBot) | Reddit 视频生成 | 2026-05-25 | GPL-3.0 | requirements、Dockerfile、Playwright | 自动化链路成熟；内容平台规则风险 |
| 12 | [soimort/you-get](https://github.com/soimort/you-get) | 网页视频下载器 | 2026-04-30 | NOASSERTION | requirements、setup、ffmpeg | 素材入口强；许可证和平台规则需确认 |
| 13 | [yt-dlp/yt-dlp](https://github.com/yt-dlp/yt-dlp) | 强力媒体下载器 | 2026-05-25 | Unlicense | Python、FFmpeg | 媒体采集首选；平台条款风险 |
| 14 | [iawia002/lux](https://github.com/iawia002/lux) | 快速视频下载 | 2026-03-29 | MIT | Go | 简洁下载工具；覆盖面需对比 yt-dlp |
| 15 | [opentoonz/opentoonz](https://github.com/opentoonz/opentoonz) | 二维动画制作 | 2026-05-26 | NOASSERTION | 桌面依赖 | 动画制作入口；不是 AI 自动化工具 |
| 16 | [zhouxiaoka/autoclip](https://github.com/zhouxiaoka/autoclip) | 自动剪辑工具 | 2026-05-08 | MIT | requirements、Docker、FastAPI、React、FFmpeg | 自动剪辑可验证；部署较重 |
| 17 | [browser-use/video-use](https://github.com/browser-use/video-use) | 浏览器视频代理 | 2026-05-15 | MIT | pyproject、ffmpeg、remotion | 浏览器视频代理方向新；成熟度需实测 |
| 18 | [HKUDS/ViMax](https://github.com/HKUDS/ViMax) | 视频多模态模型 | 2026-05-26 | MIT | pyproject | 研究价值高；落地需二次工程化 |
| 19 | [facebookresearch/pytorchvideo](https://github.com/facebookresearch/pytorchvideo) | 视频理解研究库 | 2026-05-05 | Apache-2.0 | Python、Torch | 视频理解研究可用；不是生成工具 |
| 20 | [PaddlePaddle/PaddleVideo](https://github.com/PaddlePaddle/PaddleVideo) | 视频理解工具箱 | 2025-02-12 | Apache-2.0 | Python、Paddle | 中文生态可参考；活跃度一般 |
| 21 | [XPixelGroup/BasicSR](https://github.com/XPixelGroup/BasicSR) | 视频图像修复 | 2024-07-21 | Apache-2.0 | Python、Torch | 修复/超分基础库；维护偏旧 |
| 22 | [PeterL1n/BackgroundMattingV2](https://github.com/PeterL1n/BackgroundMattingV2) | 视频背景抠像 | 2024-06-19 | MIT | requirements、Torch | 抠像方向实用；维护偏旧 |
| 23 | [AliaksandrSiarohin/first-order-model](https://github.com/AliaksandrSiarohin/first-order-model) | 图像驱动动画 | 2024-11-14 | MIT | requirements、Dockerfile、ffmpeg | 经典研究项目；新项目需评估替代方案 |
| 24 | [chatfire-AI/huobao-drama](https://github.com/chatfire-AI/huobao-drama) | 火爆短剧系统 | 2026-05-21 | 未声明 | Docker、ffmpeg、Node、OpenAI、Vue | 短剧场景明确；许可证不清 |
| 25 | [alecm20/story-flicks](https://github.com/alecm20/story-flicks) | 故事视频生成 | 2025-03-12 | 未声明 | pyproject、docker-compose、FastAPI、OpenAI、React | 场景可参考；许可证不清 |
| 26 | [yuanzhongqiao/deep-comedy-pro](https://github.com/yuanzhongqiao/deep-comedy-pro) | 短剧喜剧生成 | 2026-05-10 | 未声明 | 未发现明显运行依赖 | 早期项目；需验证质量 |
| 27 | [happyhorseai/happyhorse](https://github.com/happyhorseai/happyhorse) | AI 视频项目 | 2026-04-08 | 未声明 | 未发现明显运行依赖 | 可观察；成熟度和授权不清 |
| 28 | [ltaoo/wx_channels_download](https://github.com/ltaoo/wx_channels_download) | 视频号下载器 | 2026-05-24 | NOASSERTION | go.mod | 视频号素材入口；平台规则风险 |
| 29 | [jianshuo/claude-skills](https://github.com/jianshuo/claude-skills) | Claude 技能合集 | 2026-05-26 | MIT；API 可能收费 | 有代码依赖 | 技能参考；不是视频工具内核 |
| 30 | [TencentARC/VQFR](https://github.com/TencentARC/VQFR) | 人脸视频修复 | 2022-12-15 | NOASSERTION | Python/模型 | 可作修复参考；维护较旧 |

## 四、自媒体

| 推荐 | 项目 | 简介 | 最后更新 | 许可/付费 | 外部依赖 | 推荐理由 / 风险 |
|---:|---|---|---:|---|---|---|
| 1 | [yt-dlp/yt-dlp](https://github.com/yt-dlp/yt-dlp) | 强力媒体下载器 | 2026-05-25 | Unlicense | Python、FFmpeg | 素材采集首选；需遵守平台条款 |
| 2 | [firecrawl/firecrawl](https://github.com/firecrawl/firecrawl) | 网页转 AI 数据 | 2026-05-26 | AGPL-3.0 | Node/服务端依赖 | 网页内容结构化强；AGPL 和服务成本需注意 |
| 3 | [D4Vinci/Scrapling](https://github.com/D4Vinci/Scrapling) | 智能网页抓取 | 2026-05-18 | BSD-3-Clause | pyproject、Dockerfile | 采集能力强、许可清晰 |
| 4 | [browser-use/browser-use](https://github.com/browser-use/browser-use) | 浏览器自动化代理 | 2026-05-26 | MIT | Python、浏览器、LLM | 可处理复杂网页流程；账号风控要重视 |
| 5 | [langchain-ai/langchain](https://github.com/langchain-ai/langchain) | 智能体开发平台 | 2026-05-26 | MIT | Python/JS 生态 | 内容生成和工具编排生态强；框架复杂度高 |
| 6 | [Comfy-Org/ComfyUI](https://github.com/Comfy-Org/ComfyUI) | 节点式生成工作流 | 2026-05-26 | GPL-3.0 | requirements、pyproject | 图片素材生产强；部署成本较高 |
| 7 | [harry0703/MoneyPrinterTurbo](https://github.com/harry0703/MoneyPrinterTurbo) | AI 短视频生成 | 2026-05-26 | MIT | Python、Docker、OpenAI | 短视频生产首选验证项 |
| 8 | [elebumm/RedditVideoMakerBot](https://github.com/elebumm/RedditVideoMakerBot) | Reddit 视频自动化 | 2026-05-25 | GPL-3.0 | Python、Docker、Playwright | 自动化链路完整；内容平台风险 |
| 9 | [soimort/you-get](https://github.com/soimort/you-get) | 网页媒体下载 | 2026-04-30 | NOASSERTION | Python、FFmpeg | 素材下载常用；授权需核实 |
| 10 | [iawia002/lux](https://github.com/iawia002/lux) | 快速视频下载 | 2026-03-29 | MIT | Go | 简洁备选 |
| 11 | [Panniantong/Agent-Reach](https://github.com/Panniantong/Agent-Reach) | 营销触达代理 | 2026-05-18 | MIT | pyproject | 营销触达方向明确；需注意合规和平台风控 |
| 12 | [yikart/AiToEarn](https://github.com/yikart/AiToEarn) | AI 赚钱导航 | 2026-05-21 | MIT | docker-compose、Node | 适合找项目线索；不是生产框架 |
| 13 | [joeseesun/qiaomu-anything-to-notebooklm](https://github.com/joeseesun/qiaomu-anything-to-notebooklm) | 资料转 NotebookLM | 2026-04-28 | MIT | requirements | 内容整理实用；依赖 NotebookLM 工作流 |
| 14 | [mvanhorn/last30days-skill](https://github.com/mvanhorn/last30days-skill) | 近 30 天热点追踪 | 2026-05-22 | MIT | pyproject、Anthropic、OpenAI | 热点追踪可用；API 成本另算 |
| 15 | [KKKKhazix/khazix-skills](https://github.com/KKKKhazix/khazix-skills) | 内容技能合集 | 2026-05-08 | MIT；API 可能收费 | 有代码依赖 | 内容流程可参考；需筛选质量 |
| 16 | [op7418/Humanizer-zh](https://github.com/op7418/Humanizer-zh) | 中文 AI 降痕 | 2026-01-19 | MIT | 未发现明显运行依赖 | 文案处理可参考；效果需实测 |
| 17 | [huangserva/skill-prompt-generator](https://github.com/huangserva/skill-prompt-generator) | 技能提示生成 | 2026-05-10 | 未声明 | requirements、OpenAI | 提示词生成可参考；许可证不清 |
| 18 | [CheeMao/ai-content](https://github.com/CheeMao/ai-content) | AI 内容平台 | 2026-03-20 | NOASSERTION | docker-compose、Next.js、OpenAI、React | 内容平台方向；许可证不清 |
| 19 | [jackwener/xiaohongshu-cli](https://github.com/jackwener/xiaohongshu-cli) | 小红书命令行 | 2026-03-21 | 未声明 | pyproject | 小红书场景明确；账号和平台风控高 |
| 20 | [hekaixin66-sketch/xiaohongshuritter](https://github.com/hekaixin66-sketch/xiaohongshuritter) | 小红书采集工具 | 2026-04-05 | 未声明 | go.mod、Dockerfile | 采集场景明确；授权和平台规则风险 |

## 五、金融

| 推荐 | 项目 | 简介 | 最后更新 | 许可/付费 | 外部依赖 | 推荐理由 / 风险 |
|---:|---|---|---:|---|---|---|
| 1 | [OpenBB-finance/OpenBB](https://github.com/OpenBB-finance/OpenBB) | 金融数据平台 | 2026-05-26 | NOASSERTION | Python/数据源 | 投研数据入口强；数据源可能收费 |
| 2 | [microsoft/qlib](https://github.com/microsoft/qlib) | AI 量化平台 | 2026-04-22 | MIT | Python、数据源 | AI 量化研究首选之一 |
| 3 | [vnpy/vnpy](https://github.com/vnpy/vnpy) | 量化交易框架 | 2026-05-17 | MIT | Python、交易接口 | 中文量化生态成熟；实盘接入需严格风控 |
| 4 | [mementum/backtrader](https://github.com/mementum/backtrader) | 策略回测框架 | 2024-08-19 | GPL-3.0 | Python | 回测经典；维护偏旧、GPL 约束 |
| 5 | [freqtrade/freqtrade](https://github.com/freqtrade/freqtrade) | 加密交易机器人 | 2026-05-26 | GPL-3.0 | Python、交易所 API | 加密策略验证成熟；实盘风险高 |
| 6 | [TauricResearch/TradingAgents](https://github.com/TauricResearch/TradingAgents) | 多智能体交易 | 2026-05-17 | Apache-2.0 | requirements、pyproject、Docker、Anthropic、OpenAI | Agent 投研代表项目；先做研究别直接实盘 |
| 7 | [Open-Dev-Society/OpenStock](https://github.com/Open-Dev-Society/OpenStock) | 开源股票平台 | 2026-05-02 | AGPL-3.0 | package.json、Docker、Next.js、Node | 股票平台形态完整；AGPL 和部署成本 |
| 8 | [ZhuLinsen/daily_stock_analysis](https://github.com/ZhuLinsen/daily_stock_analysis) | 每日股票分析 | 2026-05-26 | MIT | requirements、pyproject、FastAPI、OpenAI | 日常分析自动化可参考 |
| 9 | [HKUDS/Vibe-Trading](https://github.com/HKUDS/Vibe-Trading) | 情绪交易代理 | 2026-05-25 | MIT | pyproject、Docker、FastAPI、React | 情绪交易方向活跃；需严谨回测 |
| 10 | [polakowo/vectorbt](https://github.com/polakowo/vectorbt) | 向量化回测 | 2026-04-25 | NOASSERTION | Python | 快速策略研究；授权需核实 |
| 11 | [pmorissette/bt](https://github.com/pmorissette/bt) | 组合回测工具 | 2026-05-05 | MIT | Python | 组合回测轻量；生态不如主流平台 |
| 12 | [TA-Lib/ta-lib-python](https://github.com/TA-Lib/ta-lib-python) | 技术指标库 | 2026-03-16 | BSD-2-Clause | TA-Lib 本体 | 指标计算基础库；不是完整平台 |
| 13 | [quantopian/zipline](https://github.com/quantopian/zipline) | 量化回测库 | 2024-02-13 | Apache-2.0 | Python | 经典回测框架；更新偏旧 |
| 14 | [binance/binance-connector-python](https://github.com/binance/binance-connector-python) | 币安 API 连接器 | 2026-05-22 | MIT | Python、Binance API | 交易所接口清晰；交易所和地区合规风险 |
| 15 | [okx/agent-trade-kit](https://github.com/okx/agent-trade-kit) | OKX 交易工具包 | 2026-05-20 | MIT | package.json、OKX | Agent 交易工具方向；实盘风险高 |
| 16 | [Fincept-Corporation/FinceptTerminal](https://github.com/Fincept-Corporation/FinceptTerminal) | 金融终端框架 | 2026-05-26 | NOASSERTION | Dockerfile | 终端框架方向；许可证不清 |
| 17 | [brokermr810/QuantDinger](https://github.com/brokermr810/QuantDinger) | 量化投研工具 | 2026-05-25 | Apache-2.0 | docker-compose | 投研工具可观察；成熟度需实测 |
| 18 | [anthropics/financial-services](https://github.com/anthropics/financial-services) | 金融 AI 示例 | 2026-05-21 | Apache-2.0 | 有代码依赖 | 示例参考价值高；不是完整产品 |
| 19 | [virattt/dexter](https://github.com/virattt/dexter) | 数据分析代理 | 2026-05-24 | 未声明 | package.json、Anthropic、OpenAI | 数据分析 Agent 可参考；许可证不清 |
| 20 | [koala73/worldmonitor](https://github.com/koala73/worldmonitor) | 全球信息监控 | 2026-05-26 | NOASSERTION | package.json、Docker、docker-compose | 宏观信息监控可参考；许可证不清 |

## 六、设计

| 推荐 | 项目 | 简介 | 最后更新 | 许可/付费 | 外部依赖 | 推荐理由 / 风险 |
|---:|---|---|---:|---|---|---|
| 1 | [shadcn-ui/ui](https://github.com/shadcn-ui/ui) | 开源组件集合 | 2026-05-25 | MIT | React、Tailwind | 现代前端组件首选之一 |
| 2 | [ant-design/ant-design](https://github.com/ant-design/ant-design) | 企业 React 组件 | 2026-05-26 | MIT | React | 企业后台成熟度高 |
| 3 | [mui/material-ui](https://github.com/mui/material-ui) | Material 组件库 | 2026-05-25 | MIT | React | 国际化生态强 |
| 4 | [tailwindlabs/tailwindcss](https://github.com/tailwindlabs/tailwindcss) | 原子化 CSS 框架 | 2026-05-24 | MIT | Node/CSS 工具链 | 快速搭建 UI 体系 |
| 5 | [storybookjs/storybook](https://github.com/storybookjs/storybook) | 组件开发文档 | 2026-05-26 | MIT | Node、前端框架 | 组件工程化和设计系统必备 |
| 6 | [penpot/penpot](https://github.com/penpot/penpot) | 开源设计工具 | 2026-05-26 | MPL-2.0 | Web/服务端依赖 | 开源 Figma 替代方向 |
| 7 | [nexu-io/open-design](https://github.com/nexu-io/open-design) | 开放设计平台 | 2026-05-26 | Apache-2.0；API 可能收费 | package.json、OpenAI | AI 设计平台方向活跃 |
| 8 | [plasmicapp/plasmic](https://github.com/plasmicapp/plasmic) | 可视化 React 构建 | 2026-05-25 | MIT | React/平台依赖 | 可视化构建能力强；平台绑定需评估 |
| 9 | [webstudio-is/webstudio](https://github.com/webstudio-is/webstudio) | 开源网站构建器 | 2026-05-26 | AGPL-3.0 | Web 技术栈 | 网站构建器方向；AGPL 约束 |
| 10 | [BuilderIO/gpt-crawler](https://github.com/BuilderIO/gpt-crawler) | 站点知识抓取 | 2025-07-07 | ISC | Node | 可为设计/站点重构准备上下文 |
| 11 | [figma/plugin-samples](https://github.com/figma/plugin-samples) | Figma 插件示例 | 2026-03-23 | MIT | Figma API | 插件开发参考 |
| 12 | [VoltAgent/awesome-design-md](https://github.com/VoltAgent/awesome-design-md) | 设计提示合集 | 2026-05-18 | MIT | 未发现明显运行依赖 | 提示资产价值高；不是工具 |
| 13 | [JCodesMore/ai-website-cloner-template](https://github.com/JCodesMore/ai-website-cloner-template) | AI 网站克隆模板 | 2026-05-07 | MIT；API 可能收费 | package.json、Docker、Anthropic、Next.js、OpenAI、React | 站点克隆工作流可参考；依赖 SaaS/API |
| 14 | [nextlevelbuilder/ui-ux-pro-max-skill](https://github.com/nextlevelbuilder/ui-ux-pro-max-skill) | UIUX 提示技能 | 2026-04-03 | MIT | 有代码依赖 | UI 提示流程可参考 |

## 七、编程 & Agent

| 推荐 | 项目 | 简介 | 最后提交 | 许可/付费 | 外部依赖 | 推荐理由 / 风险 |
|---:|---|---|---:|---|---|---|
| 1 | [openai/codex](https://github.com/openai/codex) | 终端编程 Agent | 未在原文记录 | 开源；模型另付 | 终端、本地仓库、OpenAI | 编程 Agent 工作流核心入口 |
| 2 | [All-Hands-AI/OpenHands](https://github.com/All-Hands-AI/OpenHands) | 软件工程 Agent 平台 | 未在原文记录 | 开源；模型另付 | Docker/浏览器/LLM | 软件工程 Agent 平台成熟度高 |
| 3 | [bytedance/deer-flow](https://github.com/bytedance/deer-flow) | 长任务超级 Agent | 2026-05-26 | MIT；模型另付 | Makefile；Python/Node | 长任务、子代理、记忆、沙箱架构完整 |
| 4 | [openclaw/openclaw](https://github.com/openclaw/openclaw) | 本地个人 AI 助理 | 2026-05-26 | MIT；模型另付 | Node/PNPM、多扩展 | 个人数据自托管和多通道集成好 |
| 5 | [microsoft/autogen](https://github.com/microsoft/autogen) | 多 Agent 编排框架 | 未在原文记录 | 开源；模型另付 | Python/.NET/LLM | 多 Agent 编排生态强 |
| 6 | [langchain-ai/langgraph](https://github.com/langchain-ai/langgraph) | 状态图 Agent 框架 | 未在原文记录 | 开源；模型另付 | Python/JS、LangChain | 可控 Agent 流程编排强 |
| 7 | [crewAIInc/crewAI](https://github.com/crewAIInc/crewAI) | 角色协作 Agent 框架 | 未在原文记录 | 开源；模型另付 | Python、LLM | 角色协作上手快；复杂任务需验证 |
| 8 | [nousresearch/hermes-agent](https://github.com/nousresearch/hermes-agent) | 自学习个人 Agent | 2026-05-25 | MIT；模型/API 另付 | agent-browser、OpenAI、httpx、rich | 技能学习和个人助理形态完整 |
| 9 | [browser-use/browser-use](https://github.com/browser-use/browser-use) | 浏览器 Agent 自动化 | 2026-05-26 | MIT | 浏览器、LLM | Web 任务自动化强；账号风控高 |
| 10 | [simular-ai/agent-s](https://github.com/simular-ai/agent-s) | 桌面控制 Agent | 2026-05-13 | Apache-2.0；API 另付 | OpenAI、Anthropic、FastAPI、PaddleOCR | CUA 实用性强；桌面权限风险高 |
| 11 | [affaan-m/ECC](https://github.com/affaan-m/ECC) | Agent 操作系统 | 2026-05-25 | MIT；模型另付 | Node/Python、Anthropic、OpenAI | 覆盖技能、规则、MCP、安全 |
| 12 | [obra/superpowers](https://github.com/obra/superpowers) | Agent 技能方法论 | 2026-05-04 | MIT | 轻量 package.json | 跨 Claude、Codex、OpenCode 的流程资产 |
| 13 | [addyosmani/agent-skills](https://github.com/addyosmani/agent-skills) | 工程技能集合 | 2026-05-24 | MIT | 无 manifest | 工程质量门槛和流程成熟 |
| 14 | [anthropics/skills](https://github.com/anthropics/skills) | Claude 官方技能集 | 2026-05-19 | 未声明许可证 | 无 manifest | 标准参考价值高；商用复用需谨慎 |
| 15 | [MiniMax-AI/skills](https://github.com/MiniMax-AI/skills) | MiniMax 技能集合 | 2026-04-18 | 有 LICENSE | 技能文件 | 国产模型技能参考 |
| 16 | [vercel-labs/skills](https://github.com/vercel-labs/skills) | Vercel 技能集合 | 2026-05-23 | 免费；需核实 | 技能文件 | 技能发现和模板参考 |
| 17 | [HKUDS/OpenSpace](https://github.com/HKUDS/OpenSpace) | GUI 智能体空间 | 2026-05-21 | MIT；API 另付 | litellm、OpenAI、MCP、Anthropic | 软件操作泛化研究价值高 |
| 18 | [HKUDS/CLI-Anything](https://github.com/HKUDS/CLI-Anything) | 软件转 CLI | 2026-05-23 | Apache-2.0 | 无 manifest | 扩展 Agent 可操作软件范围 |
| 19 | [paperclipai/paperclip](https://github.com/paperclipai/paperclip) | 业务运行 Agent | 2026-05-25 | MIT；模型另付 | Playwright、esbuild、TypeScript | 面向业务流程自动化 |
| 20 | [thunlp/ProactiveAgent](https://github.com/thunlp/ProactiveAgent) | 主动事件 Agent | 2026-05-12 | Apache-2.0；API 另付 | OpenAI、tiktoken、pynput、aw-client | 主动 Agent 学术参考 |
| 21 | [davila7/claude-code-templates](https://github.com/davila7/claude-code-templates) | Claude 配置模板 CLI | 2026-05-26 | MIT；云服务另付 | Supabase、Vercel Postgres、Axios | 模板和监控一体；SaaS 依赖多 |
| 22 | [hesamsheikh/octogent](https://github.com/hesamsheikh/octogent) | 多代理编程看板 | 2026-04-20 | MIT；模型另付 | Node、node-pty、ws、TypeScript | 多 Claude/Codex 会话管理 |
| 23 | [ruvnet/ruflo](https://github.com/ruvnet/ruflo) | Claude Flow 工作流 | 2026-05-26 | MIT | @claude-flow、zod、WASM | 工作流与 MCP 结合紧 |
| 24 | [code-yeongyu/oh-my-openagent](https://github.com/code-yeongyu/oh-my-openagent) | OpenAgent 工具套件 | 2026-05-26 | Sustainable Use License | MCP SDK、OpenCode、ast-grep | 面向多 Harness；许可证限制更强 |
| 25 | [EveryInc/compound-engineering-plugin](https://github.com/EveryInc/compound-engineering-plugin) | 复合工程插件 | 2026-05-24 | MIT | citty、js-yaml、semantic-release | 工程流程插件化 |
| 26 | [farion1231/cc-switch](https://github.com/farion1231/cc-switch) | 多 Agent 配置切换 | 2026-05-26 | MIT | CodeMirror、Dnd Kit | 多 CLI 配置管理；不是 Agent 内核 |
| 27 | [kepano/obsidian-skills](https://github.com/kepano/obsidian-skills) | Obsidian Agent 技能 | 2026-05-24 | MIT | 无 manifest | 知识库自动化好 |
| 28 | [K-Dense-AI/claude-scientific-skills](https://github.com/K-Dense-AI/claude-scientific-skills) | 科研 Agent 技能 | 2026-05-25 | MIT；抓取服务可能另付 | firecrawl-py、python-dotenv | 科研场景专业 |
| 29 | [mattpocock/skills](https://github.com/mattpocock/skills) | 工程师常用技能 | 2026-05-20 | MIT | 无 manifest | TypeScript 工程经验强 |
| 30 | [ant-design/antd-skill](https://github.com/ant-design/antd-skill) | Ant Design 技能 | 2026-03-27 | MIT | 轻量 package.json | 前端设计规范技能 |
| 31 | [antvis/chart-visualization-skills](https://github.com/antvis/chart-visualization-skills) | 图表可视化技能 | 2026-05-25 | MIT | commander、gray-matter、TypeScript | 数据可视化 Agent 技能 |
| 32 | [coreyhaines31/marketingskills](https://github.com/coreyhaines31/marketingskills) | 营销 Agent 技能 | 2026-05-21 | MIT | 无 manifest | 垂直营销流程清晰 |
| 33 | [tinyhumansai/openhuman](https://github.com/tinyhumansai/openhuman) | 开源数字人助手 | 2026-05-26 | GPL-3.0 | Tauri、Rive、Rust/Cargo | 交互形态新；GPL 约束 |
| 34 | [karpathy/autoresearch](https://github.com/karpathy/autoresearch) | 自动化 AI 研究 | 2026-03-25 | 未声明许可证；算力另付 | numpy、pandas、tiktoken、requests | 概念影响力强；授权和稳定性不足 |
| 35 | [AndyMik90/Aperant](https://github.com/AndyMik90/Aperant) | 多代理编码框架 | 2026-03-23 | AGPL-3.0 | React/lucide、jsdom | 计划-构建-验证闭环；AGPL 约束 |
| 36 | [iamzhihuix/skills-manage](https://github.com/iamzhihuix/skills-manage) | Skills 桌面管理器 | 2026-05-02 | Apache-2.0 | Tauri、Base UI、LobeHub icons | 技能管理层；不是执行框架 |
| 37 | [nicedreamzapp/claude-code-local](https://github.com/nicedreamzapp/claude-code-local) | 本地模型跑 Claude | 2026-05-22 | MIT | 无 manifest | 本地隐私方向；依赖硬件/模型 |
| 38 | [multica-ai/andrej-karpathy-skills](https://github.com/multica-ai/andrej-karpathy-skills) | Karpathy 编码准则 | 2026-04-20 | 未声明许可证 | 无 manifest | 单文件易复制；授权需谨慎 |
| 39 | [Donchitos/Claude-Code-Game-Studios](https://github.com/Donchitos/Claude-Code-Game-Studios) | Claude 游戏团队 | 2026-05-13 | MIT | 无 manifest | 游戏开发流程模板 |
| 40 | [msitarzewski/agency-agents](https://github.com/msitarzewski/agency-agents) | AI 专家角色库 | 2026-04-11 | MIT | 无 manifest | 角色覆盖广；不是可运行框架 |
| 41 | [jnMetaCode/agency-agents-zh](https://github.com/jnMetaCode/agency-agents-zh) | 中文专家角色库 | 2026-05-19 | MIT | 轻量 package.json | 中文本地化好；依赖上游内容 |

## 八、浏览器 / 桌面自动化 / 工具底座

| 推荐 | 项目 | 简介 | 最后提交 | 许可/付费 | 外部依赖 | 推荐理由 / 风险 |
|---:|---|---|---:|---|---|---|
| 1 | [simular-ai/agent-s](https://github.com/simular-ai/agent-s) | 桌面控制 Agent | 2026-05-13 | Apache-2.0；API 另付 | OpenAI、Anthropic、FastAPI、PaddleOCR | 桌面 CUA 首选验证项 |
| 2 | [TurixAI/TuriX-CUA](https://github.com/TurixAI/TuriX-CUA) | 桌面动作模型 | 2026-05-25 | MIT | pyautogui、pynput、Pillow、rapidfuzz | 桌面动作执行明确 |
| 3 | [browser-use/browser-harness](https://github.com/browser-use/browser-harness) | 浏览器控制 Harness | 2026-05-20 | MIT | cdp-use、fetch-use、Pillow、websockets | 浏览器自动化基础好 |
| 4 | [vercel-labs/agent-browser](https://github.com/vercel-labs/agent-browser) | Agent 浏览器 CLI | 2026-05-20 | Apache-2.0 | package.json、Rust CLI | 快速浏览器自动化 |
| 5 | [openclaw/Peekaboo](https://github.com/openclaw/Peekaboo) | Mac 屏幕自动化 | 2026-05-25 | MIT | chrome-devtools-mcp | macOS GUI 操作实用 |
| 6 | [microsoft/playwright](https://github.com/microsoft/playwright) | 浏览器自动化基础库 | 未在原文记录 | Apache-2.0 | Node/Python/Java/.NET | Web 自动化标准工具 |
| 7 | [puppeteer/puppeteer](https://github.com/puppeteer/puppeteer) | Chrome 自动化库 | 未在原文记录 | Apache-2.0 | Node、Chrome | Chrome 自动化成熟 |
| 8 | [SeleniumHQ/selenium](https://github.com/SeleniumHQ/selenium) | WebDriver 生态 | 未在原文记录 | Apache-2.0 | 多语言、浏览器驱动 | 企业兼容性强 |
| 9 | [modelcontextprotocol/servers](https://github.com/modelcontextprotocol/servers) | MCP 工具服务器集合 | 未在原文记录 | 开源；需核实 | 多服务依赖 | Agent 工具扩展入口 |
| 10 | [public-apis/public-apis](https://github.com/public-apis/public-apis) | 免费 API 目录 | 2026-05-26 | MIT | 无 manifest | 可给 Agent 扩工具源 |
| 11 | [googleworkspace/cli](https://github.com/googleworkspace/cli) | Google Workspace CLI | 2026-03-31 | Apache-2.0；Google API 账号 | Node/Rust、changesets、Cargo | 办公套件可被 Agent 调用 |
| 12 | [Tencent/openclaw-weixin](https://github.com/Tencent/openclaw-weixin) | OpenClaw 微信插件 | 2026-05-18 | MIT 文本 | openclaw、zod、silk-wasm、qrcode | 微信通道价值高；登录和合规约束 |
| 13 | [clawvader-tech/hermes-telegram-miniapp](https://github.com/clawvader-tech/hermes-telegram-miniapp) | Hermes 聊天前端 | 2026-04-15 | MIT | 无 manifest | Telegram 入口清晰；需配后端 |
| 14 | [antirez/ds4](https://github.com/antirez/ds4) | DeepSeek 本地引擎 | 2026-05-26 | MIT | Makefile/C | 小型本地推理引擎清晰 |
| 15 | [Mininglamp-AI/cider](https://github.com/Mininglamp-AI/cider) | MLX 量化推理 | 2026-05-11 | MIT | MLX、numpy | macOS/MLX 优化；非 Agent 应用 |
| 16 | [AndrewNgGirl/SkillLens](https://github.com/AndrewNgGirl/SkillLens) | Skill 质量评估 | 2026-05-17 | MIT | 无 manifest | 适合筛选技能库；成熟度需验证 |
| 17 | [kangarooking/cangjie-skill](https://github.com/kangarooking/cangjie-skill) | 书籍方法论技能 | 2026-05-04 | MIT | 无 manifest | 内容型技能可复用；非工程框架 |
| 18 | [FujiwaraChoki/MoneyPrinterV2](https://github.com/FujiwaraChoki/MoneyPrinterV2) | 自动视频生成 | 2026-05-15 | AGPL-3.0；平台/API 可能另付 | requests、schedule、kittentts、webdriver | 自动化链路完整；AGPL 与平台风控风险 |

## 九、官网 / 产品页 / 非单仓库入口

这些链接不是可直接评估的单一 GitHub 仓库，建议只作为产品或组织入口，再按具体仓库、价格、许可和数据合规单独确认。

| 推荐 | 链接 | 简介 | 状态 | 判断 |
|---:|---|---|---|---|
| 1 | [Marvis](https://marvis.qq.com/) | 腾讯系统级助手 | 官网 2026-05 可下载 | 闭源，本地/云端模型和桌面权限需确认 |
| 2 | [CodeBuddy WorkBuddy](https://www.codebuddy.cn/work/) | 腾讯办公 Agent | 定价页 2026-05-15 后生效 | 商业产品，个人专业版 58 元/月，企业版 198/316 元/月起 |
| 3 | [QoderWake](https://qoder.com/qoderwake) | 24 小时数字员工 | 官网可访问；未见仓库 | 闭源云产品，需信任平台 |
| 4 | [Helio](https://www.helio.im/) | AI 原生团队工作区 | 官网可访问 | 闭源，团队协作平台 |
| 5 | [Clockless AI](https://clockless.ai/) | 客户关系 AI 门户 | 官网可访问 | 闭源 SaaS，需销售确认 |
| 6 | [ClawinLink](https://claw.baolieguoshi.com/) | Agent 消息网关 | 官网内测 | 微信/QQ 通道，合规和接入门槛高 |
| 7 | [ghuntley](https://github.com/ghuntley) | Agent 方法论作者 | 个人主页 | 不是单仓库，适合看其教程和代表仓库 |
| 8 | [TauricResearch](https://github.com/TauricResearch) | 金融 Agent 组织 | GitHub 组织主页 | 应按组织内具体仓库评估 |
| 9 | [Binance](https://github.com/binance) | Binance 组织 | GitHub 组织主页 | 应按具体 SDK/接口仓库评估 |
| 10 | [OpenToonz 官网](https://opentoonz.github.io/e/index.html) | 开源二维动画软件 | 官网入口 | GitHub 仓库应看 opentoonz/opentoonz |
| 11 | [yikeai](https://www.yikeai.com/#/home) | 商业 AI 视频平台 | 官网入口 | 非仓库，价格和素材授权需确认 |
| 12 | [Wind 金融技能页](https://aifinmarket.wind.com.cn/skill.md) | Wind 金融技能页 | 页面入口 | 商业数据/服务属性需确认 |
| 13 | [MCPMarket UI Prompt Generator](https://mcpmarket.com/zh/tools/skills/ui-prompt-generator) | UI 提示工具页 | 页面入口 | 非仓库，无法按开源许可判断 |
| 14 | [腾讯 ArDot](https://ardot.tencent.com/) | 腾讯设计平台 | 官网入口 | 非仓库，商业和平台绑定需确认 |

## 十、需重点复核的条目

| 条目 | 原因 | 建议 |
|---|---|---|
| `NVIDIA/DanceDiffusion` | GitHub API 返回 404 | 可能仓库名写错、未公开或已迁移，先不要纳入推荐 |
| `YadiraF/ClothFlow` | GitHub API 返回 404 | 只查到论文/项目页线索，需重新确认公开仓库 |
| `NOASSERTION` / 未声明许可证条目 | 无法确认商用复用边界 | 商业项目中不要直接复制代码，先查 LICENSE、模型权重和依赖许可证 |
| 换脸、人脸识别、桌面控制、浏览器控制、微信/QQ 通道 | 涉及隐私、账号、平台规则和误操作风险 | 必须做权限隔离、日志审计、人工确认和合规边界 |
| 金融交易 Agent / 交易所 SDK | 容易被误用为实盘自动交易 | 先做研究、回测、模拟盘；实盘需要风控和合规审查 |
