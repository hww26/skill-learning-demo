# skill-learning-demo
概念学习资料生成Skill练习仓库

## 《大数据与人工智能》课程作业
本仓库用于《大数据与人工智能》课程作业的提交与版本管理，本次作业实现一套可复用的概念学习资料生成Skill，并产出Agent、大模型上下文、Skill三份学习资料与三者关系文档。

### 目录结构skill-learning-demo/
├── README.md                 # 本说明文档
├── .gitignore                # Git忽略规则
├── .workbuddy/
│   └── skills/
│       └── concept-learning-generator/
│           └── SKILL.md      # 项目级通用概念学习资料生成Skill
├── learning-materials/       # Skill生成并人工核验后的学习资料
│   ├── agent.html
│   ├── llm-context.html
│   ├── skill.html
│   └── concept-relationship.html
├── hw01/                     # 第一次作业
└── notebooks/                # Jupyter 笔记本 / 数据分析实验 
### Skill说明
- Skill名称：`concept-learning-generator`
- Skill存放路径：`.workbuddy/skills/concept-learning-generator/SKILL.md`
- 调用方式：在WorkBuddy中，使用指令 `使用 concept-learning-generator 生成【概念名】的学习资料`，输入任意AI专业概念即可产出结构化学习文档
- Skill能力：通用概念生成，可输出个人理解、核心机制、应用场景、概念边界、可核验参考链接

### 本次作业已生成资料清单
1. learning-materials/agent.html — Agent 概念学习资料
2. learning-materials/llm-context.html — 大模型上下文 概念学习资料
3. learning-materials/skill.html — Skill 概念学习资料
4. learning-materials/concept-relationship.html — Agent、上下文、Skill三者关系说明

###  人工核查与修改记录
1. 调用Skill生成初稿后，重写【个人理解】板块，改为学习者自己的表述，不直接复用AI原始文本
2. 逐一核验参考链接，剔除无效、404链接，保留公开可访问的权威来源
3. 补充完善每个概念的落地应用场景、易混淆误区与使用边界
4. 在关系文档中梳理上下文窗口对Agent推理的约束、Skill如何沉淀可复用任务知识

### 作业列表
| 作业 | 内容 | 状态 |
| ---- | ---- | ---- |
| hw01 | 概念学习Skill + Agent/上下文/Skill学习资料 | 已完成 |

### 使用约定
- 每次作业放在独立的 `hwXX/` 目录中，代码与报告一起提交
- 数据文件较大时不要直接推送到GitHub，使用网盘/学校服务器链接并在README中注明