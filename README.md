# Tang · AI Application & Quality Engineering

关注 AI 应用工程、RAG 评测、后端与质量工程。这里记录项目的实现、设计取舍与可复查的验证结果。

## 项目

| 项目 | 一句话说明 | 主要技术 | 入口 |
| --- | --- | --- | --- |
| [商品影棚](https://github.com/asifours-blip/shangpin-yingpeng) | 将商品资料、内容生成、人工审核和素材交付连接为可追踪的运营流程。 | FastAPI、Vue 3、PostgreSQL、Redis、MinIO | [使用流程](https://github.com/asifours-blip/shangpin-yingpeng#运营人员怎么用) · [工程案例](https://github.com/asifours-blip/shangpin-yingpeng/blob/main/docs/engineering-cases.md) |
| [智能客服与工单协作平台](https://github.com/asifours-blip/ai-customer-service-agent) | 将知识问答、售后确认、客服处理和反馈评测串联，业务权限与副作用由后端校验。 | FastAPI、LangGraph、PostgreSQL / pgvector | [项目说明](https://github.com/asifours-blip/ai-customer-service-agent) · [并发案例](https://github.com/asifours-blip/ai-customer-service-agent/blob/main/docs/ticket-concurrency-case-study.md) |
| [RAG Quality Lab](https://github.com/asifours-blip/llm-evaluation-playground) | 分开检查检索、回答、拒答与成本，保存实验记录并比较逐题结果。 | Python、SQLite、BM25、Jinja2 | [项目说明](https://github.com/asifours-blip/llm-evaluation-playground) · [数据集说明](https://github.com/asifours-blip/llm-evaluation-playground/blob/main/docs/dataset-v1.1-review.md) |
| [农产品溯源系统](https://github.com/asifours-blip/traceability-system) | 连接生产、分销、零售与消费者查询，记录批次交接、链上状态及对应文件。 | Spring Boot、Vue 2、FISCO BCOS、IPFS | [项目说明](https://github.com/asifours-blip/traceability-system) · [运行记录](https://github.com/asifours-blip/traceability-system/blob/master/docs/artifacts/README.md) |

## 工程原则

- 分别衡量功能、成本和证据质量，让结论对应具体的验证范围。
- 将权限和不可逆的业务操作放在确定性代码里，不交给模型提示词决定。
- 优先保留可复现的具体回归，避免依赖宽泛而无法核查的声明。

各项目的离线测试、本地隔离验证与真实接入状态分别写在仓库文档中。
