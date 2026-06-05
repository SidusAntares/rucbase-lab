## Lab2: Buffer Pool Manager

### 实现概述
<!-- 简述核心设计思路，如替换算法选择、并发控制策略 -->

### 关键设计决策
- **为什么选 Clock 而非 LRU？**：...
- **页表锁粒度**：选择了 per-page latch 而非全局锁，因为...

### 测试与验证
- [x] 通过所有提供的 GTest 用例
- [x] 自定义边界测试：连续驱逐同一帧...
- 性能基准：YCSB-A 吞吐量 xxx ops/s

### 已知问题 / TODO
- 当前未处理 flush 失败的回滚逻辑

### 关联 Commits
<!-- 可选：列出关键节点的 commit hash -->
