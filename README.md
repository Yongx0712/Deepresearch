# 🧠 HelloAgents-DeepResearch
# （AI 深度研究智能体）
基于 HelloAgents 框架构建的 AI 深度研究智能体，支持自动联网搜索、信息分析、研究报告一站式生成 ✨

# 🎯 项目介绍
这是我自主开发的深度研究智能体项目，能够根据用户输入的研究主题，自动完成问题拆解、资料搜索、内容归纳、报告生成全流程工作。

# ✨ 核心功能
- 🤖 AI 自动拆解研究问题
- 🌐 联网搜索获取最新资料
- 🧩 多轮信息整合与验证
- 📝 自动生成 Markdown 研究报告
- 🛠️ 模块化设计，易于扩展

# 📁 项目结构
```bash
helloagents-deepresearch/
├── .vscode/              # 编辑器配置
│   └── settings.json
├── backend/              # 后端主目录
│   ├── src/              # 后端源码
│   │   ├── services/     # 业务服务模块
│   │   │   ├── __init__.py
│   │   │   ├── notes.py
│   │   │   ├── planner.py
│   │   │   ├── reporter.py
│   │   │   ├── search.py
│   │   │   ├── summarizer.py
│   │   │   ├── text_processing.py
│   │   │   └── tool_events.py
│   │   ├── __init__.py
│   │   ├── agent.py      # AI 智能体核心
│   │   ├── config.py     # 配置文件
│   │   ├── main.py       # 程序入口
│   │   ├── models.py     # 数据模型
│   │   ├── prompts.py    # 提示词模板
│   │   └── utils.py      # 工具函数
│   ├── .env              # 环境变量
│   ├── requirements.txt  # 后端依赖
│   ├── pyproject.toml    # 项目配置
│   └── uv.lock           # 依赖锁
├── frontend/             # 前端主目录
│   ├── src/              # 前端源码
│   │   ├── services/
│   │   │   └── api.ts    # 接口请求
│   │   ├── App.vue
│   │   ├── env.d.ts
│   │   ├── main.ts
│   │   └── style.css
│   ├── .env.local        # 前端环境变量
│   ├── .gitignore
│   ├── index.html        # 页面入口
│   ├── package-lock.json
│   ├── package.json      # 前端依赖配置
│   ├── tsconfig.json     # TS 配置
│   ├── tsconfig.node.json
│   └── vite.config.ts    # 构建配置
└── README.md             # 项目说明文档
```

# 🚀 安装与使用

## 1. 进入项目目录
```bash
cd F:\helloagents-deepresearch
```

## 2. 创建虚拟环境
```bash
运行
python -m venv venv
venv\Scripts\activate
```

## 3. 后端安装依赖
```bash
运行
pip install -r requirements.txt
```

## 4. 前端安装依赖
```bash
运行
cd frontend
npm install
```

## 5. 配置 API Key
```bash
env
LLM_API_KEY=你的API密钥
LLM_BASE_URL=https://api.deepseek.com/v1
LLM_MODEL_NAME=deepseek-chat
TAVILY_API_KEY=你的搜索密钥
```

## 6. 运行项目
```bash
运行
python backend/main.py
```


📌 使用说明  
运行后输入你想研究的主题，AI 会自动：  
- 拆解问题  
- 搜索资料  
- 整合信息  
- 生成研究报告  
