# Tang · AI Application & Quality Engineering

你好，我是 Tang，主要做 AI 应用工程、RAG 评测和后端开发。

我比较在意的是：一个 AI 系统上线之后，能不能说清楚它哪里做得好、哪里做得不好、花了多少钱、出了问题能不能追溯到原因。

## 项目

### [商品影棚](https://github.com/asifours-blip/shangpin-yingpeng)
电商内容运营工作台：从商品资料出发，生成抖音和小红书的内容，经过人工审核后交付素材。重点处理了定时任务并发、审核版本锁定，以及发布结果不确定时怎么办。
`FastAPI` `Vue 3` `PostgreSQL` `Redis` `MinIO`  · [工程案例](https://github.com/asifours-blip/shangpin-yingpeng/blob/main/docs/engineering-cases.md)

### [智能客服与工单协作平台](https://github.com/asifours-blip/ai-customer-service-agent)
售后客服 Agent：知识问答附带引用，售后资格由规则判定，办理前需要客户确认，然后交给客服处理工单。模型只负责理解和表达，权限与写操作都由后端把关。
`FastAPI` `LangGraph` `PostgreSQL` `pgvector` · [并发问题排查记录](https://github.com/asifours-blip/ai-customer-service-agent/blob/main/docs/ticket-concurrency-case-study.md)

### [RAG Quality Lab](https://github.com/asifours-blip/llm-evaluation-playground)
RAG 评测工具：把检索、回答、拒答和成本分开度量，每次实验都可复现、可逐题对比；预算预检覆盖每一次外部调用，实验中断后可以续跑。
`Python` `SQLite` `BM25` · [实验发现](https://github.com/asifours-blip/llm-evaluation-playground#它帮我发现了什么)

### [农产品溯源系统](https://github.com/asifours-blip/traceability-system)
基于 FISCO BCOS 联盟链的溯源平台。原本是我的毕业设计，后来发现它的安全模型有根本性问题，就整体重新设计了身份、合约权限和交易状态管理。
`Spring Boot` `Vue 2` `Solidity` `FISCO BCOS` `IPFS` · [重新设计的经过](https://github.com/asifours-blip/traceability-system#从毕业设计到重新设计)

## 我做事的几个习惯

- 能力、成本和证据分开衡量，每个结论都说明它是在什么范围内验证的。
- 权限和不可逆的业务操作写在确定性的代码里，不交给提示词去决定。
- 宁可要一个小而能复现的回归测试，也不要一句宽泛却没法核实的说法。
