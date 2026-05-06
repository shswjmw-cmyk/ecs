# ecs
expert call supporting, copilot for interviewer to help summarize the key message and restructure the questionnaire.

cat > README.md << 'EOF'
# 专家访谈助手 (Expert Call Supporting)

📦 一个面向企业团队的实时用户访谈辅助 Web 工具

> 在访谈过程中，实时提供信息总结、识别信息缺口，并给出可追踪的追问建议

## 🎯 核心价值

- ✅ **实时总结**：访谈过程中自动生成回答摘要
- ✅ **智能追问**：基于上下文推荐值得追问的问题
- ✅ **信息缺口检测**：识别未覆盖的关键信息
- ✅ **标准化输出**：结构化访谈记录，方便团队复盘

## 📖 文档

| 类型 | 文档 |
|------|------|
| 📋 产品需求 | [PRD 终版](./docs/prd/PRD_v1.0_终版.md) |
| 🏗️ 技术架构 | [架构设计](./docs/architecture/技术架构_v1.0.md) |
| 💻 前端代码 | [前端原型](./docs/frontend/前端代码_v1.0.md) |
| 🔧 后端代码 | [后端原型](./docs/backend/后端代码_v1.0.md) |

## 🛠️ 技术栈

| 层级 | 技术 |
|------|------|
| 前端 | Vue 3 + Vite + Pinia + Element Plus |
| 后端 | Node.js + Express + Prisma |
| 数据库 | MySQL 8.0 |
| 缓存 | Redis 7.x |
| 部署 | 阿里云 ECS + Nginx |
| ASR | 阿里云通义听悟 |

## 🚀 快速开始

### 后端

```bash
cd backend
npm install
npx prisma generate
npx prisma migrate deploy
npm start

### 前端

cd frontend
npm install
npm run dev
