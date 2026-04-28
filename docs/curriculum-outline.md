# 课程大纲

本课程围绕一个固定案例展开：个人库存订单管理工具。

这个工具可以用几句话理解：

```text
一个人维护自己的商品和库存。
他可以创建商品规格，手动入库，创建包含多个商品的订单。
订单提交时检查并扣减库存，退单时恢复库存。
```

固定案例是为了降低入门负担。课程真正训练的是 AI coding 中的工程意识，而不是库存订单管理这个业务本身。

## 课程组织

每章采用三段式结构：

- `README.md`：本章大纲、背景和学习路径；
- `lesson.md`：学习内容、提示词对话和本章任务；
- `self-check.md`：完成检查、自检问题和复盘。

每个任务尽量走同一套闭环：

```text
需求 -> Issue -> 规格 -> 验证检查点 -> AI coding -> 反馈修正 -> diff -> commit / push -> 复盘
```

课程不会把概念当成词典讲解。很多概念只会先做最小解释，后续通过任务、提示词、报错、测试和复盘逐步加深。

## 课程大纲

### [00. Getting Started](../chapters/00-getting-started/)

建立最小 AI coding 工作方式。知道 GitHub 仓库、Git、Issue、`gh` CLI、规格、验证检查点和测试反馈的基本位置，并让 AI 创建第一个 Issue。

### [01. First Visible Page](../chapters/01-first-visible-page/)

先初始化项目，再讨论首页需求，最后实现第一个可见页面。学习者会第一次体会初始化 Issue、需求 Issue 和开发 Issue 的区别。

### [02. Product List](../chapters/02-product-list/)

做商品列表页面，理解列表、字段、空状态和加载状态。

### [03. Create Product](../chapters/03-create-product/)

增加创建商品的表单，理解输入、校验、错误提示和交互状态。

### [04. Product Spec](../chapters/04-product-spec/)

为商品增加规格信息，理解字段设计、约束和简单数据模型。

### [05. Stock In](../chapters/05-stock-in/)

实现手动入库，让商品库存增加，理解数量、状态变化和边界条件。

### [06. Data Persistence](../chapters/06-data-persistence/)

让商品、规格和库存数据在刷新后仍然存在，理解本地存储、数据库、记录和字段。

### [07. Order List](../chapters/07-order-list/)

做订单列表页面，理解订单状态、列表筛选和可追踪性。

### [08. Create Order](../chapters/08-create-order/)

创建订单，并让一个订单包含多个商品，理解关联关系、订单明细和数量。

### [09. Stock Check And Submit](../chapters/09-stock-check-and-submit/)

提交订单时检查库存，库存不足时阻止提交，库存足够时扣减库存。

### [10. Return Order](../chapters/10-return-order/)

实现退单，让退单后库存恢复，理解逆向流程、补偿和数据一致性。

### [11. API And Contracts](../chapters/11-api-and-contracts/)

把页面和数据服务分开，理解 API、请求、响应、接口契约和错误返回。

### [12. Errors And Debugging](../chapters/12-errors-and-debugging/)

故意面对错误，练习复现、定位、最小修改和验证修复。

### [13. Testing And Regression](../chapters/13-testing-and-regression/)

开始让 AI 写或运行简单测试，理解测试、回归、自动化检查和验证反馈。

### [14. Consistency And Idempotency](../chapters/14-consistency-and-idempotency/)

引入重复提交、重复下单和库存扣减问题，理解幂等、一致性和边界场景。

### [15. Refactoring](../chapters/15-refactoring/)

通过新增需求暴露早期简单实现的局限，理解重构、技术债和职责边界。

### [16. Deploy And Operate](../chapters/16-deploy-and-operate/)

让软件从本地运行走向可访问，理解部署、配置、发布和运行后反馈。

### [17. Advanced Auth And Tenant](../chapters/17-advanced-auth-and-tenant/)

进阶引入多用户、权限、多租户和数据范围，理解个人工具变成团队 SaaS 后的复杂度变化。

### [18. Review And Knowledge Base](../chapters/18-review-and-knowledge-base/)

复盘整个学习过程，把 AI coding 反馈沉淀成检查清单、提示词模板和工程判断规则。
