# 🤖 Telegram 智能 AI Agent 系统

基于大语言模型（DeepSeek）构建的对话驱动智能 Agent，接入 Telegram Bot，实现任务理解、规划与执行的自动化闭环。

---

## 📌 项目简介

本项目实现了一个可在 Telegram 中直接使用的 AI Agent 系统。  
用户通过自然语言输入任务，Agent 自动完成任务拆解（Task Planning）、内容生成（Content Generation）以及工具调用（Tool Use），并最终执行任务（如发布到 Notion）。

---

## ✨ 核心功能

- 💬 **Telegram Bot 接入**
  - 支持实时对话交互
  - 用户可通过聊天直接触发任务

- 🧠 **任务规划（Task Planning）**
  - 使用大语言模型对复杂任务进行拆解
  - 自动生成多步骤执行流程

- 🔄 **Agent 执行循环（Agent Loop）**
  - 实现「理解 → 规划 → 执行 → 反馈」闭环

- 🛠 **工具调用（Tool Use）**
  - 集成 Notion API
  - 支持内容自动发布

- 🧾 **内容生成**
  - 自动生成博客文章
  - 支持结构化输出（标题 / 段落）

- 🧠 **上下文管理**
  - 支持多轮对话
  - 提升任务执行连贯性

- 🐳 **Docker 部署**
  - 支持一键部署运行
  - 提供 API 接口供外部调用

---

## 🧩 系统架构
用户输入（Telegram）
↓
LLM（DeepSeek）
↓
Task Planner（任务拆解）
↓
Tool Executor（工具执行）
├── 内容生成
├── Notion 发布
↓
Memory（上下文）
↓
返回结果

---

## 📍 使用示例

**用户输入：**



**Agent 执行流程：**
1. 生成文章大纲
2. 撰写完整内容
3. 格式化为 Notion 页面
4. 自动发布 ✅

---

## 🛠 技术栈

- Python
- LLM API
- Telegram Bot API
- Notion API
- FastAPI
- Docker

---

## 📦 安装与运行

### 1. 克隆项目

```bash
git clone https://github.com/你的用户名/telegram-ai-agent.git
cd telegram-ai-agent
```

### 2. 安装依赖

```bash
pip install -r requirements.txt
```

### 3. 启动项目

```bash
python main.py
```

---

## 🔮 后续优化方向

* 多 Agent 架构（Planner / Executor 分离）
* RAG（接入知识库）
* Web 可视化界面
* 更复杂的工具系统（搜索 / 数据分析等）

