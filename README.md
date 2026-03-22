第 1 层：不可丢的核心记忆

放在 bootstrap/，例如：
	•	IDENTITY.md：我是谁，不是什么
	•	SOUL.md：价值观、风格、底线
	•	AGENTS.md：职责边界、协作规则
	•	TOOLS.md：允许调用什么工具，优先级是什么
	•	USER.md：关于你这个主人的长期固定认知
	•	HEARTBEAT.md：定时自检与待办规则
	•	BOOTSTRAP.md：启动时必须知道的全局准则

OpenClaw 官方已经明确这些 bootstrap 文件会自动注入 agent 上下文，并支持长度上限与总上限控制。
第 2 层：可增长的长期记忆

放在 memory/，建议做成结构化 Markdown 仓库：
memory/
├── 00-principles.md
├── 01-user-profile.md
├── 02-goals.md
├── 03-projects.md
├── 04-decisions.md
├── 05-contacts.md
├── 06-risks.md
└── timeline/
