# An Easy Way To Explain LLM AI

[English](#english) | [中文](#chinese)

---

<a name="english"></a>
## English

### Introduction

An interactive visualization demo that explains how Large Language Models (LLMs) work. This project uses intuitive animations and 3D visualizations to demonstrate the core mechanisms of AI language models, including the embedding layer, Transformer attention mechanism, and output prediction layer.

### Demo Preview

The demo uses a classic Chinese phrase pair as an example:
- **Input**: "天王盖地虎" (The king of heaven covers the earth tiger)
- **Output**: "宝塔镇河妖" (The pagoda suppresses the river demon)

This is a famous call-and-response phrase from Chinese culture, perfect for demonstrating how LLMs predict the next token based on context.

### Features

- **2D Flowchart Mode**: Step-by-step visualization of the LLM processing pipeline
  - Input & Embedding Layer: Shows how text is converted to vectors with positional encoding
  - Transformer Layer: Visualizes attention weights between tokens
  - Output Layer: Displays probability distribution and token selection

- **3D Vector Space Mode**: Interactive 3D visualization using Three.js
  - Drag to rotate the view
  - Scroll to zoom in/out
  - Watch attention connections flow between tokens
  - See candidate tokens positioned in semantic space

### How It Works

1. **Embedding Layer (Step 1)**
   - Each character is converted into a high-dimensional vector
   - Positional encoding is added to preserve sequence information
   - Formula: `E(token) = Semantic Vector + Positional Encoding`

2. **Transformer Layer (Step 2)**
   - Self-attention mechanism analyzes context
   - Each token "attends to" all previous tokens
   - Attention weights determine which context is most relevant

3. **Output Layer (Step 3)**
   - Computes similarity scores for all candidate tokens
   - Softmax converts scores to probability distribution
   - Highest probability token is selected
   - Formula: `P(token) = e^(score) / Σe^(all scores)`

4. **Autoregressive Generation**
   - The selected token is appended to the input
   - Process repeats until generation is complete
   - Each iteration builds on all previous tokens

### Getting Started

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/AnEasyWayToExplainLLMAI.git
   ```

2. Open `index.html` in a modern web browser

3. Click "开始演示" (Start Demo) to begin the visualization

### File Structure

```
AnEasyWayToExplainLLMAI/
├── index.html           # Main page with tab switcher
├── ai-llm-demo.html     # 2D flowchart visualization
├── ai-llm-3d-demo.html  # 3D vector space visualization
├── three.min.js         # Three.js library for 3D rendering
└── README.md            # This file
```

### Technologies Used

- **HTML5/CSS3**: Modern styling with flexbox and grid layouts
- **Vanilla JavaScript**: No framework dependencies for core logic
- **Three.js**: 3D graphics library for vector space visualization
- **CSS Animations**: Smooth transitions and visual feedback

### Browser Support

- Chrome (recommended)
- Firefox
- Safari
- Edge

### License

GPLv3

---

<a name="chinese"></a>
## 中文

### 项目简介

这是一个交互式可视化演示项目，用于解释大语言模型（LLM）的工作原理。本项目通过直观的动画和3D可视化，展示AI语言模型的核心机制，包括嵌入层、Transformer注意力机制和输出预测层。

### 演示预览

演示使用经典中国俗语对子作为示例：
- **输入**: "天王盖地虎"
- **输出**: "宝塔镇河妖"

这是中国文化中著名的"接头暗号"，非常适合用来演示LLM如何根据上下文预测下一个词元。

### 功能特点

- **2D流程图模式**：逐步可视化LLM处理流程
  - 输入与嵌入层：展示文字如何转换为带位置编码的向量
  - Transformer层：可视化词元之间的注意力权重
  - 输出层：显示概率分布和词元选择过程

- **3D向量空间模式**：使用Three.js的交互式3D可视化
  - 拖动旋转视角
  - 滚轮缩放
  - 观看注意力连接在词元之间流动
  - 查看候选词元在语义空间中的位置

### 工作原理

1. **嵌入层（第一步）**
   - 每个字符被转换成高维向量
   - 添加位置编码以保留序列信息
   - 公式：`E(字符) = 语义向量 + 位置编码`

2. **Transformer层（第二步）**
   - 自注意力机制分析上下文
   - 每个词元"关注"所有前面的词元
   - 注意力权重决定哪些上下文最相关

3. **输出层（第三步）**
   - 计算所有候选词元的相似度分数
   - Softmax将分数转换为概率分布
   - 选择概率最高的词元
   - 公式：`P(字) = e^(分数) / Σe^(所有分数)`

4. **自回归生成**
   - 选中的词元被添加到输入序列
   - 重复上述过程直到生成完成
   - 每次迭代都基于所有已有词元

### 快速开始

1. 克隆仓库：
   ```bash
   git clone https://github.com/yourusername/AnEasyWayToExplainLLMAI.git
   ```

2. 在现代浏览器中打开 `index.html`

3. 点击"开始演示"按钮开始可视化

### 文件结构

```
AnEasyWayToExplainLLMAI/
├── index.html           # 主页面，包含标签切换器
├── ai-llm-demo.html     # 2D流程图可视化
├── ai-llm-3d-demo.html  # 3D向量空间可视化
├── three.min.js         # Three.js 3D渲染库
└── README.md            # 本文件
```

### 技术栈

- **HTML5/CSS3**：使用flexbox和grid的现代布局
- **原生JavaScript**：核心逻辑无框架依赖
- **Three.js**：用于向量空间可视化的3D图形库
- **CSS动画**：流畅的过渡和视觉反馈

### 浏览器支持

- Chrome（推荐）
- Firefox
- Safari
- Edge

### 许可证

GPLv3

---

## Contributing | 贡献

Contributions are welcome! Please feel free to submit a Pull Request.

欢迎贡献！请随时提交 Pull Request。
