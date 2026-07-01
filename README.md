# 认知外骨骼系统 · Cognitive Exoskeleton System

> **用哲学作为解释工具、用结构化规则约束思维、并强制导向现实行动的认知外骨骼系统**

---

## 🚀 快速启动

### GitHub Pages 部署

1. 创建 GitHub 仓库（如 cognitive-exoskeleton）
2. 将本仓库的 docs/ 目录内容推送至 main 分支
3. 在仓库 Settings → Pages 中：
   - Source: **Deploy from a branch**
   - Branch: main, folder: /docs
4. 等待 2-3 分钟后访问 https://<你的用户名>.github.io/<仓库名>/

### 直接使用

打开 docs/index.html 即可在本地使用（需联网调用 DeepSeek API）

---

## 🧠 系统架构

`mermaid
flowchart LR
    U[用户输入] --> C[Chat Interface]
    C --> API[DeepSeek API]
    API --> P[认知外骨骼引擎]
    P --> S[Sidebar Visualization]
    KB[哲学知识库<br/>42部经典著作] -.-> P
    S --> T[State Timeline]
    S --> PA[Pattern Detection]
    S --> PH[Philosophy References]
    S --> AC[Action Items]
    S --> RM[Risk Monitor]
`

---

## 📚 哲学知识库

系统内置了从 Project Gutenberg 获取的 **42部经典哲学著作**，涵盖 19 位哲学家：

| 类别 | 哲学家 | 著作数 |
|------|--------|--------|
| 🟢 解释类 | 现象学、系统论、结构主义 | - |
| 🟡 决策辅助类 | 实用主义、存在主义 | - |
| 🔵 认知纠偏类 | 维特根斯坦、笛卡尔、海德格尔 | - |
| 📐 理性主义 | Descartes | 1 |
| 🧩 语言哲学 | Wittgenstein | 1 |
| 🦁 存在主义 | Nietzsche, Kierkegaard | 11 |
| 🇺🇸 实用主义 | William James | 3 |
| 🏛️ 古典 | Plato, Aristotle | 7 |
| 🇩🇪 德国观念论 | Kant, Hegel, Schopenhauer | 5 |
| 🇫🇷 社会哲学 | Rousseau, Marx | 5 |
| 🇬🇧 经验主义/功利主义 | Hume, Mill, Berkeley | 5 |
| 🏛️ 斯多葛 | Marcus Aurelius, Epictetus | 2 |
| ✝️ 中世纪 | Augustine | 1 |

---

## ⚙️ 配置

在 docs/index.html 中搜索 C.key 可修改 API Key：

`javascript
var C = {
    key: "sk-your-api-key-here",
    model: "deepseekv4-flash",
    url: "https://api.deepseek.com/v1/chat/completions"
};
`

---

## 🎯 核心功能

- **认知状态追踪**：实时识别 🟢 行动态 / 🟡 内省态 / 🔴 循环态
- **模式识别引擎**：检测 10+ 种常见认知模式（分析瘫痪、完美启动、自我审查等）
- **哲学分析模块**：受控使用现象学、实用主义、存在主义等工具
- **行动约束系统**：强制生成具体、可执行、非思考类的下一步行动
- **风险监控**：持续追踪内耗、拖延、决策延迟等风险指标

---

## 📄 许可

MIT License

知识库文本来自 [Project Gutenberg](https://www.gutenberg.org/)，遵循公共领域许可。
