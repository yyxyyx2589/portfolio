# 作品集 · 余毅轩

AI Agent 应用开发方向求职作品集。三个开源项目围绕同一个问题：
**当模型不确定时，Agent 该怎么决策** —— 用检索置信度做路由信号，决定「直答 / 走工具循环 / 拒答转人工」。

**在线页面：<https://yyxyyx2589.github.io/portfolio/>**

## 收录的作品

| 作品 | 仓库 | 一句话 |
|---|---|---|
| 银行远程坐席知识助手 | [bank-agent](https://github.com/yyxyyx2589/bank-agent) | RAG 三级置信度路由 + ReAct 双引擎编排 + 自建银行域 LoRA。三基线（Agent 100% / 纯 RAG 69.8% / 本地 1.5B+LoRA 66.7%）+ 消融证明 LoRA 净增 +7.2 点 |
| 企业 IT 运维智能体 | [ops-agent](https://github.com/yyxyyx2589/ops-agent) | 把 RAG 检索置信度升级为决策路由信号的原始实现；手写 ReAct 与 LangGraph 双编排，10 场景等价性可验证 |
| 小红书公开内容监控 Agent | [xhs_monitor](https://github.com/yyxyyx2589/xhs_monitor) | 确定性执行流 + 风险自适应调度 + 规则/LLM 混合分析；评测暴露出现有分析器意图任务漏接率 100% |

配套技术长文：[《瓶颈不是模型大小，是知识边界》](https://github.com/yyxyyx2589/bank-agent/blob/main/docs/%E6%8A%80%E6%9C%AF%E5%A4%8D%E7%9B%98.md)（约 3900 字，六个真踩过的坑）

## 本地查看

单文件、零依赖，直接用浏览器打开即可：

```bash
start index.html        # Windows
open  index.html        # macOS
```

## 关于内容

- 页面里引用的所有数字均可在对应仓库的 `README`、`reports/` 与测试中复核。
- 三个项目都是**可复现的演示原型**：数据由脚本生成或取自公开页面，不代表线上生产表现。
  各项目的诚实边界写在它自己的 README 与页面的「诚实边界」一节里。
- `bank-agent` 是 `ops-agent` 的同构换皮（转移的是方法，不是两个从零的独立项目）——这一点在页面上也如实标注。

## 许可证

[MIT](LICENSE)
