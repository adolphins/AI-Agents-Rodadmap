# 🧱 阶段一：编程基石与数据处理 (Python & Backend)

> *"A building is only as strong as its foundation."*  
> 本阶段的目标是夯实 Python 编程底座，掌握大模型开发中必不可少的后端 API 搭建与快速 Web UI 构建能力。

---

## 🎯 核心目标

- [ ] 掌握 Python 高阶特性（OOP、装饰器、多并发），告别只会写简单脚本的“小白”阶段。  
- [ ] 能够使用 **FastAPI** 独立编写 RESTful API 接口。  
- [ ] 掌握 **Pandas** 等工具进行基础的数据清洗（这对后续 RAG 知识库构建处理文档极为重要）。  
- [ ] 熟练使用 **Streamlit**，能为 AI 模型快速套上美观的网页外壳。

---

## 📚 优质学习资源推荐

> 资源很多，不必全看，根据自己基础挑选 1–2 个认真跟完即可。

### 🎥 视频教程（Bilibili / YouTube）

| 类别 | 推荐课程 | 说明 |
|------|----------|------|
| **Python 语法与进阶** | [黑马程序员 - Python 全套教程](https://www.bilibili.com/video/BV1qW4y1a7fU)（B站） | 超详细版，适合查漏补缺 |
| | [Corey Schafer - Python OOP Tutorials](https://www.youtube.com/playlist?list=PL-osiE80TeTsqhIuOqKhwlXsIBIdSeYtc)（YouTube） | 公认最好的面向对象系列（英文） |
| | [freeCodeCamp - OOP with Python](https://www.youtube.com/watch?v=Ej_02ICOIgs)（YouTube） | 新版 OOP 实战 |
| **后端 API 开发 (FastAPI)** | [黑马程序员 - Python Web 开发](https://www.bilibili.com/video/BV1zV2QBtE39)（B站） | 基础到实战 |
| | [freeCodeCamp - FastAPI Course](https://www.youtube.com/watch?v=0sOvCWFmrtA)（YouTube） | 构建 RESTful API |
| | [FastAPI Full Course（核心系列）](https://www.youtube.com/watch?v=iukOehU5aF4)（YouTube） | 全栈 Web App 实战 |
| **数据分析 (Pandas)** | [Python for Data Science Course](https://www.youtube.com/watch?v=GPVsHOlRBBI)（YouTube） | Pandas 基础 |
| | [EDA + AB测试实战](https://www.youtube.com/watch?v=FTpmwX94_Yo)（YouTube） | 项目驱动 |
| | [freeCodeCamp - Data Science](https://www.youtube.com/watch?v=ua-CiDNNj30)（可选） | 综合合集 |
| **Web 可视化 (Streamlit)** | [12 Data Science Apps with Streamlit](https://www.youtube.com/watch?v=JwSS70SZdyM)（YouTube） | 快速上手 |
| | [Streamlit 30天挑战](https://30daysofai.streamlit.app/)（官网） | 每日一练 |
| | [Building web apps using Streamlit](https://www.youtube.com/watch?v=3YGBqEt4rRE)（YouTube） | 实战教程 |

### 📖 必读书籍

| 封面 | 书名与说明 |
|------|-------------|
| 📘 | **《Learning Python》** (6th Edition)<br>*Powerful Object-Oriented Programming* —— 入门必备，实战性强 |
| 📗 | **《Fluent Python》** (2nd Edition)<br>*Clear, Concise, and Effective Programming* —— 进阶神书！重点看装饰器、生成器、并发部分 |
| 📕 | **《Python for Data Analysis》** (3rd Edition)<br>*Data Wrangling with pandas, NumPy, and Jupyter* —— Pandas 作者亲笔，适合当作工具书查阅 |
| 📙 | **《Build a Large Language Model》** (From Scratch)<br>*深入 LLM 底层实现* —— 适合与阶段三配合阅读 |
| 📒 | **《Hands-On Machine Learning with Scikit-Learn, Keras, and TensorFlow》** (3rd Edition)<br>*经典 ML 实战* —— 可选，为后续深度学习打底 |

### 🔗 实用工具与网站

- [FastAPI 官方中文文档](https://fastapi.tiangolo.com/zh/) – 业界良心，比很多教程都易懂  
- [Streamlit 官方文档](https://docs.streamlit.io/) – 查询各种 UI 组件（按钮、聊天框等）的首选  
- [Reddit 好帖汇总](https://www.reddit.com/r/Python/comments/103i4d2/what_are_the_best_books_to_learn_python/) – 社区推荐的 Python 学习书籍讨论

---

## 💻 练习与代码记录

> 本文件夹下的学习进度与代码位置，完成一项请勾选 ✅

- [ ] **`01_python_advanced/` – 语法进阶**  
  - [ ] 面向对象练习（类、继承、多态、魔法方法）  
  - [ ] 装饰器原理与实战（`@property`、计时器装饰器等）  
  - [ ] 迭代器与生成器（`yield` 关键字）

---

## 🏆 阶段实战项目：简易对话机器人 (Basic Chatbot)

**项目位置：** `02_basic_chatbot/`

### 项目说明

整合本阶段所学，使用 Python 调用任意大模型开放 API（例如 OpenAI / 智谱 GLM / DeepSeek），并利用 Streamlit 构建一个类似 ChatGPT 的网页聊天端。

### 核心要求

- ✅ 能够输入问题并得到模型回复  
- ✅ 支持多轮对话（上下文记忆）  
- ✅ 界面简洁，至少包含“发送”按钮和聊天记录显示区  

### 扩展挑战（可选）

- 🔧 增加对话历史清空按钮  
- 🔧 支持切换不同模型（如从 DeepSeek 切换到 智谱 GLM）  
- 🔧 实现流式输出（打字机效果）

---

<div align="center">
  
**🐍 打好地基，才能盖起摩天大厦 —— 阶段一加油！**

⭐️ 如果你完成了本阶段，欢迎回到根目录打卡并进入阶段二。

</div>