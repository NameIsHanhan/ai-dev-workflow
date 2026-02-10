# 🚀 AI 智能化研发体系落地方案

> **适用对象**：B2C / 网赚类产品 / 短剧 · 12人研发团队
> **目标**：交付周期↓20% · BUG↓20% · 人效↑30%
> **核心抓手**：AI IDE（TRAE / Cursor）全流程嵌入 + 标准化文档→任务包转换机制

---

## 📋 项目结构

```
ai-dev-workflow/
├── README.md                          # 项目总览
├── .cursorrules                       # 项目级 AI 规则文件
│
├── docs/
│   ├── overview/
│   │   ├── A-one-page-summary.md      # A. 一页纸总览
│   │   ├── B-organization.md          # B. 组织与职责
│   │   └── C-e2e-process.md           # C. 端到端流程
│   │
│   ├── templates/                     # D. 交付物与模板目录
│   │   ├── T001-PRD-template.md
│   │   ├── T002-tech-design-backend.md
│   │   ├── T003-tech-design-frontend.md
│   │   ├── T004-tech-design-android.md
│   │   ├── T005-page-spec.md
│   │   ├── T006-api-spec.md
│   │   ├── T007-task-package-backend.md
│   │   ├── T008-task-package-frontend.md
│   │   ├── T009-task-package-android.md
│   │   ├── T010-test-case.md
│   │   ├── T011-release-checklist.md
│   │   ├── T012-rollback-plan.md
│   │   ├── T013-retrospective.md
│   │   └── T014-prompt-log.md
│   │
│   ├── task-conversion/               # E. 文档→任务包转换机制
│   │   ├── E-conversion-mechanism.md
│   │   └── examples/
│   │       ├── TASK-BE-001-checkin.yaml
│   │       ├── TASK-FE-001-checkin.yaml
│   │       ├── TASK-AD-001-checkin.yaml
│   │       └── TASK-QA-001-checkin.yaml
│   │
│   ├── prompts/                       # F. AI IDE Prompt 体系
│   │   ├── F0-context-rules.md
│   │   ├── master/F1-master-prompts.md
│   │   ├── product/F2-product-prompts.md
│   │   ├── ui/F3-ui-prompts.md
│   │   ├── backend/F4-backend-prompts.md
│   │   ├── frontend/F5-frontend-prompts.md
│   │   ├── android/F6-android-prompts.md
│   │   ├── testing/F7-testing-prompts.md
│   │   ├── release/F8-release-prompts.md
│   │   └── retro/F9-retro-prompts.md
│   │
│   └── execution/                     # G. 可执行落地清单
│       └── G-execution-checklist.md
│
├── prompt-logs/                       # Prompt Log 存放目录
│   └── .gitkeep
│
└── xmind/
    └── AI智能化研发体系落地方案.md      # XMind 可导入文件
```

---

## 🎯 一页纸总览

| 维度 | 内容 |
|------|------|
| **目标** | 交付周期缩短20%；线上BUG率下降20%；人均产出提升30% |
| **范围** | 需求→方案→设计→任务拆分→开发→联调→测试→发布→复盘，全流程 |
| **关键抓手** | ① 标准化"文档→任务包"转换 ② AI IDE Prompt体系 ③ 角色协同SOP ④ Prompt Log可追溯 |
| **里程碑** | **W1-W2** 培训+工具部署 → **W3-W4** 试点1个迭代 → **W5-W8** 全量推行 → **W9-W12** 度量优化 |

## 👥 团队配置

| 角色 | 人数 | AI IDE 主要使用场景 |
|------|------|---------------------|
| 产品 | 1 | PRD结构化 → AI生成验收用例、接口草案、任务包初稿 |
| UI | 1 | AI生成页面规格文档、切图命名规范、动效参数表 |
| 后端 | 3 | AI生成Controller/Service/Mapper骨架、SQL、单测 |
| 前端(Web/H5) | 1 | AI生成页面组件、API调用层、表单校验逻辑 |
| Android | 2 | AI生成Activity/Fragment/ViewModel骨架、网络层 |
| 测试 | 3 | AI根据PRD+API文档批量生成测试用例、自动化脚本 |

## 📖 快速开始

1. **阅读总览**：`docs/overview/` 目录下 A → B → C 顺序阅读
2. **了解模板**：`docs/templates/` 目录包含所有标准化模板
3. **学习Prompt**：`docs/prompts/` 目录按角色分类的Prompt模板
4. **查看示例**：`docs/task-conversion/examples/` 目录有完整的任务包示例
5. **开始执行**：按 `docs/execution/G-execution-checklist.md` 逐步落地

## 🔧 技术栈

- **后端**：Spring Boot / Spring Cloud, MyBatis-Plus, MySQL 8.0, Redis 6.x
- **前端**：Vue 3 + TypeScript + Vite / React 18 + TypeScript + Vite
- **Android**：Kotlin, MVVM + Jetpack, Retrofit + OkHttp, Hilt
- **CI/CD**：GitLab + Jenkins
- **AI IDE**：TRAE / Cursor

---

> 📌 本方案由研发团队维护，持续迭代优化。每次迭代复盘后更新 Prompt 模板库.