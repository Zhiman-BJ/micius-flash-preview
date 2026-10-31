<div align="center">

# Micius-Flash-Preview

**知满科技 · 面向科学研究与复杂工程研发的旗舰大模型**

[![上下文](https://img.shields.io/badge/上下文-256K-01d280?style=flat-square)](https://zhiman-bj.github.io/micius-flash-preview/)
[![架构](https://img.shields.io/badge/架构-原生多模态-01d280?style=flat-square)](https://zhiman-bj.github.io/micius-flash-preview/)
[![推理](https://img.shields.io/badge/推理-深度思考-01d280?style=flat-square)](https://zhiman-bj.github.io/micius-flash-preview/)

[在线体验](https://platform.zhiman.cn/console/chat) · [API 接入](https://platform.zhiman.cn/console) · [发布页](https://zhiman-bj.github.io/micius-flash-preview/) · [知满科技官网](https://zhiman.cn/)

</div>

---

## 模型简介

**Micius（墨子）** 是知满科技推出的科学工程大模型系列，以半导体这一知识密集、工程链路复杂、专业工具高度集中的领域作为首个重点实践场景。

它是一个**懂工程、会工具、能交付**的模型：

- 🔬 **半导体知识** —— 解答工艺、器件与电路问题，并基于物理原理推理分析
- 💻 **芯片与电路代码** —— 生成可通过编译与仿真验证的 Verilog、VHDL 与 EDA 脚本
- 🤖 **工程 Agent** —— 在 EDA、KiCad 等专业工具中自主完成多步骤任务
- 👁️ **多模态理解** —— 理解电路图、原理图、版图截图与波形图等工程图像

## 核心亮点

| 亮点 | 说明 |
| --- | --- |
| **能力密度高** | 12 项硬件代码评测平均 **64.2**，较 Qwen3.8-27B 提升 15.0 分，高于 DeepSeek-V4-Pro（63.8）；半导体专项 Agent 得分 **62.41**，同样高于 DeepSeek-V4-Pro（57.29） |
| **部署门槛低** | **单张 48 GB 级专业显卡即可部署**，量化版本可运行于 24 GB 消费级显卡 |
| **数据不出域** | 支持企业内网私有化部署，满足半导体研发对设计数据安全的严格要求 |

## 技术路线

```
知识树与权威语料 → 数据合成与清洗 → 7 个领域 Teacher → 多教师在线蒸馏（MOPD）→ Micius-Flash-Preview
```

- 从 **10 个学科视角**和 **8 个产业与标准视角**分别构建半导体知识树，知识节点覆盖率 **97%+**
- **21 万+** 半导体候选问答，每道训练题都能追溯到具体出处
- 7 个领域 Teacher 先完成专项训练，再通过多教师在线蒸馏汇聚能力
- 代码与工具调用轨迹都经过**沙箱实际执行验证**，模型学到的是可运行、可验证的工程行为

## 模型规格

| 项目 | 规格 |
| --- | --- |
| 参数量 | 27B |
| 上下文长度 | 256K |
| 架构 | 原生多模态 |
| 推理 | 深度思考模式 |

## 部署

支持 vLLM、SGLang、Ollama 等主流推理框架：

| 版本 | 显卡要求 |
| --- | --- |
| FP8 | 48 GB 级专业显卡 |
| 4-bit | 24 GB 消费级显卡 |

也可通过[知满开放平台](https://platform.zhiman.cn/console) API 接入，兼容 OpenAI 与 Anthropic 接口。

## 工程演示

发布页中收录了 Micius 独立完成的真实工程任务录屏：

- **RTL-to-GDS 芯片设计** —— 自主完成逻辑综合、布局布线、时序分析和 DRC、LVS 版图验证，346 次工具调用，0 布线器 DRC 违例
- **晶体管控制板 PCB** —— 在 KiCad 中完成器件选型、原理图、布局布线与铜皮修整
- **芯片封装设计工作台** —— 以 WB-PBGA 封装为例完成"工程需求 → 专用工具 → 工程任务"闭环
- **复刻并融合工业软件** —— 自主探索 FreeCAD、Calc 与 Blender 并集成为新软件

## 相关链接

| 资源 | 状态 |
| --- | --- |
| [在线体验](https://platform.zhiman.cn/console/chat) | ✅ 已开放 |
| [API 接入](https://platform.zhiman.cn/console) | ✅ 已开放 |
| 🤗 Hugging Face 权重 | 🔜 Coming soon |
| 📄 技术报告 | 🔜 Coming soon |

---

<div align="center">
<sub>© 2026 Shanghai Zhiman Technology Co., Ltd. · Micius 取名自墨子：把知识做深，把工程做透。</sub>
</div>
