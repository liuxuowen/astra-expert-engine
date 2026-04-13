# Heartbeat Tasks

## Memory Index Maintenance
定期调用 memory_search 以触发 index sync（清理 dirty 状态）：
- 每 30 分钟检查一次记忆库是否有待同步内容
- 搜索词: "heartbeat check" 或任意轻量查询即可
- 不需要处理结果，只需触发 sync 流程