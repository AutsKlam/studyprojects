# S0 实施方案交接

Planner 已完成方案，并交给独立子仓中的 `IMPLEMENTATION.md`。完整方案留在 `projects/s0-support/IMPLEMENTATION.md`；协调者默认只读本摘要。

- 工单与资料各提供创建、列表、详情；统一输入校验，SQLite 持久化。
- React 双页签，通过 Vite 代理访问独立 FastAPI 服务。
- 前后端依赖锁定；固定种子键保证重复导入不增加同批数据。
- 后台进程隐藏启动；启动失败回滚；停止前验证进程身份及项目归属。
- 验证按 S0 任务单 A1–A6 记录，后端/脚本自测与独立浏览器验收分别报告。

交接：私有仓库 `AutsKlam/studyprojects-s0-support`，空基线 `c1252b0`，功能分支 `feat/support-workbench`。执行者只读取子仓的 `AGENTS.md`、`SPEC.md` 与 `IMPLEMENTATION.md`。

规划请求配置为 `gpt-6.1-sol / ultra`；选择理由是常规规划遵循用户最高档默认。无规划阻塞。
