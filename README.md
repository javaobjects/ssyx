<p align="center">
    <a href='https://docs.oracle.com/en/java/javase/8'><img alt="Java 8" src="./画图/Java8.png"></a>
    <a href='https://docs.spring.io/spring-boot/docs/2.6.2-SNAPSHOT/reference/html'><img alt="Spring Boot 2" src="https://img.shields.io/badge/Spring%20Boot%202-%23000000.svg?logo=springboot"></a>
    <a href='https://staging-cn.vuejs.org'><img alt="Vue 3" src="https://img.shields.io/badge/Vue%202%20-%232b3847.svg?logo=vue.js"></a><br/>
    <a href='#'><img alt="Github stars" src="https://img.shields.io/github/stars/201206030/novel?logo=github"></a>
    <a href='#'><img alt="Github forks" src="https://img.shields.io/github/forks/201206030/novel?logo=github"></a>
    <a href='#'><img alt="Gitee stars" src="https://gitee.com/novel_dev_team/novel/badge/star.svg?theme=gitee"></a>
    <a href='#'><img alt="Gitee forks" src="https://gitee.com/novel_dev_team/novel/badge/fork.svg?theme=gitee"></a>
</p>

# 尚上优选

#### 开发环境

+ Windows

#### 配置环境

| 程序           | 版本        | 说明                       |
|--------------|-----------|--------------------------|
| Jdk          | 1.8.0 161 | Java 开发工具包               |
| Mysql        | 5.5.27    | 关系型数据库                   |
| Apache-maven | 3.9.0     | Java 项目管理和构建工具           |
| Nvm          | 1.10      | Node.js 版本管理器            |
| Node         | 8.12.0    | Node.js JavaScript 运行时环境 |

#### 开发工具

| 工具                       | 版本            | 说明                      |
|--------------------------|---------------|-------------------------|
| IDEA                     | 2022.3.2      | 后前端开发IDE                |
| Git                      | 2.24.1        | 代码托管平台                  |
| Google   Chrome          | 75.0.3770.100 | 浏览器、前端调试工具              |
| Navicat                  | 11.1.13       | 数据库连接工具                 |
| Postman                  | 7.1.0         | 接口测试工具                  |
| VMware   Workstation Pro | 14.1.3        | 虚拟机(未用到或许你会用到)          |
| PowerDesigner            | 15            | 数据库设计工具(未用到或许你会用到)      |
| SQLyog                   | 12.0.3        | 数据库连接工具 (未用到或许你会用到)     |
| Visio                    | 2013          | 时序图、流程图等绘制工具(未用到或许你会用到) |
| ProcessOn                | ——            | 架构图等绘制工具(未用到或许你会用到)     |
| XMind   ZEN              | 9.2.0         | 思维导图绘制工具(未用到或许你会用到)     |
| RedisDesktop             | 0.9.3.817     | redis客户端连接工具(未用到或许你会用到) |

#### 编码规范

- 规范方式：严格遵守阿里编码规约。
- 命名统一：简介最大程度上达到了见名知意。
- 分包明确：层级分明可快速定位到代码位置。
- 注释完整：描述性高大量减少了开发人员的代码阅读工作量。
- 工具规范：使用统一jar包避免出现内容冲突。
- 代码整洁：可读性、维护性高。

#### 包的结构

```
+- ssyx -- 
|   +- .git -- 
|   +- .idea -- 
|   +- LICENSE -- 
|   +- README.md -- 
|   +- 代码 -- 
|   |   +- 01-实体类 -- 
|   |   |   +- com -- 
|   |   |   |   +- atguigu -- 
|   |   |   |   |   +- ssyx -- 
|   |   |   |   |   |   +- enums -- 
|   |   |   |   |   |   |   +- ActivityType.java -- 
|   |   |   |   |   |   |   +- BillType.java -- 
|   |   |   |   |   |   |   +- CouponRangeType.java -- 
|   |   |   |   |   |   |   +- CouponStatus.java -- 
|   |   |   |   |   |   |   +- CouponType.java -- 
|   |   |   |   |   |   |   +- OrderStatus.java -- 
|   |   |   |   |   |   |   +- PaymentStatus.java -- 
|   |   |   |   |   |   |   +- PaymentType.java -- 
|   |   |   |   |   |   |   +- ProcessStatus.java -- 
|   |   |   |   |   |   |   +- SkuType.java -- 
|   |   |   |   |   |   |   +- UserType.java -- 
|   |   |   |   |   |   +- model -- 
|   |   |   |   |   |   |   +- acl -- 
|   |   |   |   |   |   |   |   +- Admin.java -- 
|   |   |   |   |   |   |   |   +- AdminRole.java -- 
|   |   |   |   |   |   |   |   +- Permission.java -- 
|   |   |   |   |   |   |   |   +- Role.java -- 
|   |   |   |   |   |   |   |   +- RolePermission.java -- 
|   |   |   |   |   |   |   +- activity -- 
|   |   |   |   |   |   |   |   +- ActivityInfo.java -- 
|   |   |   |   |   |   |   |   +- ActivityRule.java -- 
|   |   |   |   |   |   |   |   +- ActivitySku.java -- 
|   |   |   |   |   |   |   |   +- CouponInfo.java -- 
|   |   |   |   |   |   |   |   +- CouponRange.java -- 
|   |   |   |   |   |   |   |   +- CouponUse.java -- 
|   |   |   |   |   |   |   |   +- Seckill.java -- 
|   |   |   |   |   |   |   |   +- SeckillSku.java -- 
|   |   |   |   |   |   |   |   +- SeckillSkuNotice.java -- 
|   |   |   |   |   |   |   |   +- SeckillTime.java -- 
|   |   |   |   |   |   |   +- base -- 
|   |   |   |   |   |   |   |   +- BaseEntity.java -- 
|   |   |   |   |   |   |   |   +- BaseMongoEntity.java -- 
|   |   |   |   |   |   |   |   +- MqRepeatRecord.java -- 
|   |   |   |   |   |   |   +- order -- 
|   |   |   |   |   |   |   |   +- CartInfo.java -- 
|   |   |   |   |   |   |   |   +- OrderDeliver.java -- 
|   |   |   |   |   |   |   |   +- OrderInfo.java -- 
|   |   |   |   |   |   |   |   +- OrderItem.java -- 
|   |   |   |   |   |   |   |   +- OrderLog.java -- 
|   |   |   |   |   |   |   |   +- OrderReturnApply.java -- 
|   |   |   |   |   |   |   |   +- OrderReturnReason.java -- 
|   |   |   |   |   |   |   |   +- OrderSet.java -- 
|   |   |   |   |   |   |   |   +- PaymentInfo.java -- 
|   |   |   |   |   |   |   |   +- RefundInfo.java -- 
|   |   |   |   |   |   |   +- product -- 
|   |   |   |   |   |   |   |   +- Attr.java -- 
|   |   |   |   |   |   |   |   +- AttrGroup.java -- 
|   |   |   |   |   |   |   |   +- Category.java -- 
|   |   |   |   |   |   |   |   +- Comment.java -- 
|   |   |   |   |   |   |   |   +- CommentReplay.java -- 
|   |   |   |   |   |   |   |   +- SkuAttrValue.java -- 
|   |   |   |   |   |   |   |   +- SkuImage.java -- 
|   |   |   |   |   |   |   |   +- SkuInfo.java -- 
|   |   |   |   |   |   |   |   +- SkuPoster.java -- 
|   |   |   |   |   |   |   |   +- SkuStockHistory.java -- 
|   |   |   |   |   |   |   +- search -- 
|   |   |   |   |   |   |   |   +- LeaderEs.java -- 
|   |   |   |   |   |   |   |   +- SkuEs.java -- 
|   |   |   |   |   |   |   +- sys -- 
|   |   |   |   |   |   |   |   +- Region.java -- 
|   |   |   |   |   |   |   |   +- RegionWare.java -- 
|   |   |   |   |   |   |   |   +- Ware.java -- 
|   |   |   |   |   |   |   +- user -- 
|   |   |   |   |   |   |   |   +- Driver.java -- 
|   |   |   |   |   |   |   |   +- Leader.java -- 
|   |   |   |   |   |   |   |   +- LeaderAccount.java -- 
|   |   |   |   |   |   |   |   +- LeaderBank.java -- 
|   |   |   |   |   |   |   |   +- LeaderBill.java -- 
|   |   |   |   |   |   |   |   +- LeaderUser.java -- 
|   |   |   |   |   |   |   |   +- LeaderWithdraw.java -- 
|   |   |   |   |   |   |   |   +- User.java -- 
|   |   |   |   |   |   |   |   +- UserDelivery.java -- 
|   |   |   |   |   |   |   |   +- UserLoginLog.java -- 
|   |   |   |   |   |   +- vo -- 
|   |   |   |   |   |   |   +- acl -- 
|   |   |   |   |   |   |   |   +- AdminLoginVo.java -- 
|   |   |   |   |   |   |   |   +- AdminQueryVo.java -- 
|   |   |   |   |   |   |   |   +- RoleQueryVo.java -- 
|   |   |   |   |   |   |   +- activity -- 
|   |   |   |   |   |   |   |   +- ActivityRuleVo.java -- 
|   |   |   |   |   |   |   |   +- CouponRuleVo.java -- 
|   |   |   |   |   |   |   |   +- SeckillQueryVo.java -- 
|   |   |   |   |   |   |   |   +- SeckillSkuNoticeVo.java -- 
|   |   |   |   |   |   |   |   +- SeckillSkuQueryVo.java -- 
|   |   |   |   |   |   |   |   +- SeckillSkuVo.java -- 
|   |   |   |   |   |   |   +- order -- 
|   |   |   |   |   |   |   |   +- CartInfoVo.java -- 
|   |   |   |   |   |   |   |   +- OrderConfirmVo.java -- 
|   |   |   |   |   |   |   |   +- OrderDeliverVo.java -- 
|   |   |   |   |   |   |   |   +- OrderItemMqVo.java -- 
|   |   |   |   |   |   |   |   +- OrderItemParamVo.java -- 
|   |   |   |   |   |   |   |   +- OrderMqVo.java -- 
|   |   |   |   |   |   |   |   +- OrderQueryVo.java -- 
|   |   |   |   |   |   |   |   +- OrderSubmitVo.java -- 
|   |   |   |   |   |   |   |   +- OrderUserQueryVo.java -- 
|   |   |   |   |   |   |   |   +- StockStatisticsVo.java -- 
|   |   |   |   |   |   |   +- product -- 
|   |   |   |   |   |   |   |   +- AttrGroupQueryVo.java -- 
|   |   |   |   |   |   |   |   +- CategoryQueryVo.java -- 
|   |   |   |   |   |   |   |   +- CategoryVo.java -- 
|   |   |   |   |   |   |   |   +- SkuInfoQueryVo.java -- 
|   |   |   |   |   |   |   |   +- SkuInfoVo.java -- 
|   |   |   |   |   |   |   |   +- SkuStockLockVo.java -- 
|   |   |   |   |   |   |   |   +- SkuStockVo.java -- 
|   |   |   |   |   |   |   |   +- WareQueryVo.java -- 
|   |   |   |   |   |   |   +- search -- 
|   |   |   |   |   |   |   |   +- LeaderEsQueryVo.java -- 
|   |   |   |   |   |   |   |   +- SkuEsQueryVo.java -- 
|   |   |   |   |   |   |   +- sys -- 
|   |   |   |   |   |   |   |   +- RegionVo.java -- 
|   |   |   |   |   |   |   |   +- RegionWareQueryVo.java -- 
|   |   |   |   |   |   |   +- user -- 
|   |   |   |   |   |   |   |   +- LeaderAddressVo.java -- 
|   |   |   |   |   |   |   |   +- LeaderBillQueryVo.java -- 
|   |   |   |   |   |   |   |   +- LeaderQueryVo.java -- 
|   |   |   |   |   |   |   |   +- LeaderVo.java -- 
|   |   |   |   |   |   |   |   +- UserLoginVo.java -- 
|   |   |   |   |   |   |   |   +- UserQueryVo.java -- 
|   |   |   |   |   |   |   |   +- WeixinVo.java -- 
|   |   +- 02-工具类 -- 
|   |   |   +- DateUtil.java -- 
|   |   |   +- MD5.java -- 
|   |   |   +- RedissonConfig.java -- 
|   |   |   +- 微信支付 -- 
|   |   |   |   +- ConstantPropertiesUtils.java -- 
|   |   |   |   +- HttpClient.java -- 
|   |   |   +- 计算金额工具类.txt -- 
|   |   +- 03-代码生成器 -- 
|   |   |   +- CodeGet.java -- 
|   |   |   +- 代码生成器依赖.txt -- 
|   |   +- 04-平台管理端前端代码 -- 
|   |   |   +- ssyx-admin -- 
|   |   |   |   +- .editorconfig -- 
|   |   |   |   +- .env.development -- 
|   |   |   |   +- .env.production -- 
|   |   |   |   +- .env.staging -- 
|   |   |   |   +- .eslintignore -- 
|   |   |   |   +- .eslintrc.js -- 
|   |   |   |   +- .gitignore -- 
|   |   |   |   +- .travis.yml -- 
|   |   |   |   +- babel.config.js -- 
|   |   |   |   +- build -- 
|   |   |   |   |   +- index.js -- 
|   |   |   |   +- dist -- 
|   |   |   |   |   +- favicon.ico -- 
|   |   |   |   |   +- index.html -- 
|   |   |   |   |   +- static -- 
|   |   |   |   |   |   +- css -- 
|   |   |   |   |   |   |   +- app.b7cb370e.css -- 
|   |   |   |   |   |   |   +- chunk-19a74746.9044b527.css -- 
|   |   |   |   |   |   |   +- chunk-3fa7be4f.9a9361c6.css -- 
|   |   |   |   |   |   |   +- chunk-511eaf0d.cffcae92.css -- 
|   |   |   |   |   |   |   +- chunk-5cccc9a2.3c7f5ad9.css -- 
|   |   |   |   |   |   |   +- chunk-9bf4268c.aba374f4.css -- 
|   |   |   |   |   |   |   +- chunk-e181eb12.4ad201bd.css -- 
|   |   |   |   |   |   |   +- chunk-e5d1ea66.9044b527.css -- 
|   |   |   |   |   |   |   +- chunk-elementUI.68c70ad5.css -- 
|   |   |   |   |   |   |   +- chunk-f40a34c2.3cf2ae5e.css -- 
|   |   |   |   |   |   |   +- chunk-libs.3dfb7769.css -- 
|   |   |   |   |   |   +- fonts -- 
|   |   |   |   |   |   +- img -- 
|   |   |   |   |   |   +- js -- 
|   |   |   |   +- jest.config.js -- 
|   |   |   |   +- jsconfig.json -- 
|   |   |   |   +- LICENSE -- 
|   |   |   |   +- mock -- 
|   |   |   |   |   +- index.js -- 
|   |   |   |   |   +- mock-server.js -- 
|   |   |   |   |   +- table.js -- 
|   |   |   |   |   +- user.js -- 
|   |   |   |   |   +- utils.js -- 
|   |   |   |   +- node_modules -- 
|   |   |   |   +- package-lock.json -- 
|   |   |   |   +- package.json -- 
|   |   |   |   +- postcss.config.js -- 
|   |   |   |   +- public -- 
|   |   |   |   |   +- favicon.ico -- 
|   |   |   |   |   +- index.html -- 
|   |   |   |   +- README-zh.md -- 
|   |   |   |   +- README.md -- 
|   |   |   |   +- src -- 
|   |   |   |   |   +- api -- 
|   |   |   |   |   |   +- acl -- 
|   |   |   |   |   |   |   +- permission.js -- 
|   |   |   |   |   |   |   +- role.js -- 
|   |   |   |   |   |   |   +- user.js -- 
|   |   |   |   |   |   +- activity -- 
|   |   |   |   |   |   |   +- activityInfo.js -- 
|   |   |   |   |   |   |   +- couponInfo.js -- 
|   |   |   |   |   |   |   +- seckill.js -- 
|   |   |   |   |   |   |   +- seckillSku.js -- 
|   |   |   |   |   |   |   +- seckillTime.js -- 
|   |   |   |   |   |   +- index.js -- 
|   |   |   |   |   |   +- order -- 
|   |   |   |   |   |   |   +- orderInfo.js -- 
|   |   |   |   |   |   +- product -- 
|   |   |   |   |   |   |   +- attr.js -- 
|   |   |   |   |   |   |   +- attrGroup.js -- 
|   |   |   |   |   |   |   +- category.js -- 
|   |   |   |   |   |   |   +- skuInfo.js -- 
|   |   |   |   |   |   +- sys -- 
|   |   |   |   |   |   |   +- region.js -- 
|   |   |   |   |   |   |   +- regionWare.js -- 
|   |   |   |   |   |   |   +- ware.js -- 
|   |   |   |   |   |   +- table.js -- 
|   |   |   |   |   |   +- user -- 
|   |   |   |   |   |   |   +- driver.js -- 
|   |   |   |   |   |   |   +- leader.js -- 
|   |   |   |   |   |   +- user.js -- 
|   |   |   |   |   +- App.vue -- 
|   |   |   |   |   +- assets -- 
|   |   |   |   |   |   +- 404_images -- 
|   |   |   |   |   |   |   +- 404.png -- 
|   |   |   |   |   |   |   +- 404_cloud.png -- 
|   |   |   |   |   +- components -- 
|   |   |   |   |   +- icons -- 
|   |   |   |   |   |   +- index.js -- 
|   |   |   |   |   |   +- svg -- 
|   |   |   |   |   |   |   +- dashboard.svg -- 
|   |   |   |   |   |   |   +- example.svg -- 
|   |   |   |   |   |   |   +- eye-open.svg -- 
|   |   |   |   |   |   |   +- eye.svg -- 
|   |   |   |   |   |   |   +- form.svg -- 
|   |   |   |   |   |   |   +- link.svg -- 
|   |   |   |   |   |   |   +- nested.svg -- 
|   |   |   |   |   |   |   +- password.svg -- 
|   |   |   |   |   |   |   +- table.svg -- 
|   |   |   |   |   |   |   +- tree.svg -- 
|   |   |   |   |   |   |   +- user.svg -- 
|   |   |   |   |   |   +- svgo.yml -- 
|   |   |   |   |   +- layout -- 
|   |   |   |   |   |   +- components -- 
|   |   |   |   |   |   +- index.vue -- 
|   |   |   |   |   |   +- mixin -- 
|   |   |   |   |   |   |   +- ResizeHandler.js -- 
|   |   |   |   |   +- main.js -- 
|   |   |   |   |   +- permission.js -- 
|   |   |   |   |   +- router -- 
|   |   |   |   |   |   +- index.js -- 
|   |   |   |   |   +- settings.js -- 
|   |   |   |   |   +- store -- 
|   |   |   |   |   |   +- getters.js -- 
|   |   |   |   |   |   +- index.js -- 
|   |   |   |   |   |   +- modules -- 
|   |   |   |   |   |   |   +- app.js -- 
|   |   |   |   |   |   |   +- settings.js -- 
|   |   |   |   |   |   |   +- user.js -- 
|   |   |   |   |   +- styles -- 
|   |   |   |   |   |   +- element-ui.scss -- 
|   |   |   |   |   |   +- index.scss -- 
|   |   |   |   |   |   +- mixin.scss -- 
|   |   |   |   |   |   +- sidebar.scss -- 
|   |   |   |   |   |   +- transition.scss -- 
|   |   |   |   |   |   +- variables.scss -- 
|   |   |   |   |   +- utils -- 
|   |   |   |   |   |   +- auth.js -- 
|   |   |   |   |   |   +- btn-permission.js -- 
|   |   |   |   |   |   +- get-page-title.js -- 
|   |   |   |   |   |   +- index.js -- 
|   |   |   |   |   |   +- request.js -- 
|   |   |   |   |   |   +- validate.js -- 
|   |   |   |   |   +- views -- 
|   |   |   |   |   |   +- 404.vue -- 
|   |   |   |   |   |   +- acl -- 
|   |   |   |   |   |   |   +- permission -- 
|   |   |   |   |   |   |   |   +- list.vue -- 
|   |   |   |   |   |   |   +- role -- 
|   |   |   |   |   |   |   |   +- list.vue -- 
|   |   |   |   |   |   |   |   +- roleAuth.vue -- 
|   |   |   |   |   |   |   +- user -- 
|   |   |   |   |   |   |   |   +- list.vue -- 
|   |   |   |   |   |   +- activity -- 
|   |   |   |   |   |   |   +- activityInfo -- 
|   |   |   |   |   |   |   |   +- form.vue -- 
|   |   |   |   |   |   |   |   +- list.vue -- 
|   |   |   |   |   |   |   |   +- rule.vue -- 
|   |   |   |   |   |   |   +- couponInfo -- 
|   |   |   |   |   |   |   |   +- form.vue -- 
|   |   |   |   |   |   |   |   +- list.vue -- 
|   |   |   |   |   |   |   |   +- rule.vue -- 
|   |   |   |   |   |   |   +- seckill -- 
|   |   |   |   |   |   |   |   +- list.vue -- 
|   |   |   |   |   |   |   |   +- seckillSkuList.vue -- 
|   |   |   |   |   |   |   |   +- selectTimeList.vue -- 
|   |   |   |   |   |   |   |   +- timeList.vue -- 
|   |   |   |   |   |   +- dashboard -- 
|   |   |   |   |   |   |   +- index.vue -- 
|   |   |   |   |   |   +- login -- 
|   |   |   |   |   |   |   +- index.vue -- 
|   |   |   |   |   |   +- order -- 
|   |   |   |   |   |   |   +- orderInfo -- 
|   |   |   |   |   |   |   |   +- deliverList.vue -- 
|   |   |   |   |   |   |   |   +- list.vue -- 
|   |   |   |   |   |   |   |   +- show.vue -- 
|   |   |   |   |   |   +- product -- 
|   |   |   |   |   |   |   +- attr -- 
|   |   |   |   |   |   |   |   +- form.vue -- 
|   |   |   |   |   |   |   |   +- list.vue -- 
|   |   |   |   |   |   |   +- attrGroup -- 
|   |   |   |   |   |   |   |   +- form.vue -- 
|   |   |   |   |   |   |   |   +- list.vue -- 
|   |   |   |   |   |   |   +- category -- 
|   |   |   |   |   |   |   |   +- form.vue -- 
|   |   |   |   |   |   |   |   +- list.vue -- 
|   |   |   |   |   |   |   +- skuInfo -- 
|   |   |   |   |   |   |   |   +- form.vue -- 
|   |   |   |   |   |   |   |   +- list.vue -- 
|   |   |   |   |   |   +- sys -- 
|   |   |   |   |   |   |   +- regionWare -- 
|   |   |   |   |   |   |   |   +- list.vue -- 
|   |   |   |   |   |   +- user -- 
|   |   |   |   |   |   |   +- leader -- 
|   |   |   |   |   |   |   |   +- checkList.vue -- 
|   |   |   |   |   |   |   |   +- list.vue -- 
|   |   |   |   +- tests -- 
|   |   |   |   |   +- unit -- 
|   |   |   |   |   |   +- .eslintrc.js -- 
|   |   |   |   |   |   +- components -- 
|   |   |   |   |   |   +- utils -- 
|   |   |   |   |   |   |   +- formatTime.spec.js -- 
|   |   |   |   |   |   |   +- param2Obj.spec.js -- 
|   |   |   |   |   |   |   +- parseTime.spec.js -- 
|   |   |   |   |   |   |   +- validate.spec.js -- 
|   |   |   |   +- vue.config.js -- 
|   |   +- 05-微信小程序代码 -- 
|   |   |   +- atguigu-tuan -- 
|   |   |   |   +- .DS_Store -- 
|   |   |   |   +- .gitignore -- 
|   |   |   |   +- .hbuilderx -- 
|   |   |   |   |   +- launch.json -- 
|   |   |   |   +- App.vue -- 
|   |   |   |   +- common -- 
|   |   |   |   |   +- bmap-wx.min.js -- 
|   |   |   |   |   +- const.js -- 
|   |   |   |   |   +- css -- 
|   |   |   |   |   |   +- iconfont.css -- 
|   |   |   |   |   |   +- iconfont.ttf -- 
|   |   |   |   |   |   +- iconfont.woff -- 
|   |   |   |   |   |   +- iconfont.woff2 -- 
|   |   |   |   |   +- http.api.js -- 
|   |   |   |   |   +- http.interceptor.js -- 
|   |   |   |   |   +- svgIcon.js -- 
|   |   |   |   +- components -- 
|   |   |   |   +- index.html -- 
|   |   |   |   +- main.js -- 
|   |   |   |   +- manifest.json -- 
|   |   |   |   +- node_modules -- 
|   |   |   |   +- package.json -- 
|   |   |   |   +- pages -- 
|   |   |   |   |   +- cart -- 
|   |   |   |   |   |   +- cart.vue -- 
|   |   |   |   |   +- categories -- 
|   |   |   |   |   |   +- categories.vue -- 
|   |   |   |   |   +- homeItem -- 
|   |   |   |   |   |   +- homeItem.vue -- 
|   |   |   |   |   +- index -- 
|   |   |   |   |   |   +- index.vue -- 
|   |   |   |   |   +- login -- 
|   |   |   |   |   |   +- login.vue -- 
|   |   |   |   |   +- my -- 
|   |   |   |   |   |   +- my.vue -- 
|   |   |   |   +- pages.json -- 
|   |   |   |   +- pagesLocation -- 
|   |   |   |   |   +- choosePickUpLocation -- 
|   |   |   |   |   |   +- choosePickUpLocation.vue -- 
|   |   |   |   |   +- myPickUpLocation -- 
|   |   |   |   |   |   +- myPickUpLocation.vue -- 
|   |   |   |   +- pagesOrder -- 
|   |   |   |   |   +- confirmOrder -- 
|   |   |   |   |   |   +- confirmOrder.vue -- 
|   |   |   |   |   +- getOrderInfo -- 
|   |   |   |   |   |   +- getOrderInfo.vue -- 
|   |   |   |   |   +- orderList -- 
|   |   |   |   |   |   +- orderList.vue -- 
|   |   |   |   +- pagesSeckill -- 
|   |   |   |   |   +- seckill -- 
|   |   |   |   |   |   +- seckill.vue -- 
|   |   |   |   +- static -- 
|   |   |   |   |   +- images -- 
|   |   |   |   |   +- logo.png -- 
|   |   |   |   +- store -- 
|   |   |   |   |   +- index.js -- 
|   |   |   |   |   +- modules -- 
|   |   |   |   |   |   +- cart.js -- 
|   |   |   |   |   |   +- categories.js -- 
|   |   |   |   |   |   +- index.js -- 
|   |   |   |   |   |   +- order.js -- 
|   |   |   |   |   |   +- pickUpLocation.js -- 
|   |   |   |   +- uni.scss -- 
|   |   |   |   +- unpackage -- 
|   |   |   |   |   +- dist -- 
|   |   |   |   |   |   +- dev -- 
|   |   |   |   |   |   |   +- .automator -- 
|   |   |   |   |   |   |   |   +- mp-weixin -- 
|   |   |   |   |   |   |   |   |   +- .automator.json -- 
|   |   |   |   |   |   |   +- .sourcemap -- 
|   |   |   |   |   |   |   |   +- mp-weixin -- 
|   |   |   |   |   |   |   |   |   +- common -- 
|   |   |   |   |   |   |   |   |   |   +- main.js.map -- 
|   |   |   |   |   |   |   |   |   |   +- runtime.js.map -- 
|   |   |   |   |   |   |   |   |   |   +- vendor.js.map -- 
|   |   |   |   |   |   |   |   |   +- components -- 
|   |   |   |   |   |   |   |   |   +- node-modules -- 
|   |   |   |   |   |   |   |   |   |   +- uview-ui -- 
|   |   |   |   |   |   |   |   |   |   |   +- components -- 
|   |   |   |   |   |   |   |   |   +- pages -- 
|   |   |   |   |   |   |   |   |   |   +- cart -- 
|   |   |   |   |   |   |   |   |   |   |   +- cart.js.map -- 
|   |   |   |   |   |   |   |   |   |   +- categories -- 
|   |   |   |   |   |   |   |   |   |   |   +- categories.js.map -- 
|   |   |   |   |   |   |   |   |   |   +- homeItem -- 
|   |   |   |   |   |   |   |   |   |   |   +- homeItem.js.map -- 
|   |   |   |   |   |   |   |   |   |   +- index -- 
|   |   |   |   |   |   |   |   |   |   |   +- index.js.map -- 
|   |   |   |   |   |   |   |   |   |   +- login -- 
|   |   |   |   |   |   |   |   |   |   |   +- login.js.map -- 
|   |   |   |   |   |   |   |   |   |   +- my -- 
|   |   |   |   |   |   |   |   |   |   |   +- my.js.map -- 
|   |   |   |   |   |   |   |   |   +- pagesLocation -- 
|   |   |   |   |   |   |   |   |   |   +- choosePickUpLocation -- 
|   |   |   |   |   |   |   |   |   |   |   +- choosePickUpLocation.js.map -- 
|   |   |   |   |   |   |   |   |   |   +- myPickUpLocation -- 
|   |   |   |   |   |   |   |   |   |   |   +- myPickUpLocation.js.map -- 
|   |   |   |   |   |   |   |   |   +- pagesOrder -- 
|   |   |   |   |   |   |   |   |   |   +- confirmOrder -- 
|   |   |   |   |   |   |   |   |   |   |   +- confirmOrder.js.map -- 
|   |   |   |   |   |   |   |   |   |   +- getOrderInfo -- 
|   |   |   |   |   |   |   |   |   |   |   +- getOrderInfo.js.map -- 
|   |   |   |   |   |   |   |   |   |   +- orderList -- 
|   |   |   |   |   |   |   |   |   |   |   +- orderList.js.map -- 
|   |   |   |   |   |   |   |   |   +- pagesSeckill -- 
|   |   |   |   |   |   |   |   |   |   +- seckill -- 
|   |   |   |   |   |   |   |   |   |   |   +- seckill.js.map -- 
|   |   |   |   |   |   |   +- mp-weixin -- 
|   |   |   |   |   |   |   |   +- app.js -- 
|   |   |   |   |   |   |   |   +- app.json -- 
|   |   |   |   |   |   |   |   +- app.wxss -- 
|   |   |   |   |   |   |   |   +- common -- 
|   |   |   |   |   |   |   |   |   +- main.js -- 
|   |   |   |   |   |   |   |   |   +- main.wxss -- 
|   |   |   |   |   |   |   |   |   +- runtime.js -- 
|   |   |   |   |   |   |   |   |   +- vendor.js -- 
|   |   |   |   |   |   |   |   +- components -- 
|   |   |   |   |   |   |   |   +- node-modules -- 
|   |   |   |   |   |   |   |   |   +- uview-ui -- 
|   |   |   |   |   |   |   |   |   |   +- components -- 
|   |   |   |   |   |   |   |   +- pages -- 
|   |   |   |   |   |   |   |   |   +- cart -- 
|   |   |   |   |   |   |   |   |   |   +- cart.js -- 
|   |   |   |   |   |   |   |   |   |   +- cart.json -- 
|   |   |   |   |   |   |   |   |   |   +- cart.wxml -- 
|   |   |   |   |   |   |   |   |   |   +- cart.wxss -- 
|   |   |   |   |   |   |   |   |   +- categories -- 
|   |   |   |   |   |   |   |   |   |   +- categories.js -- 
|   |   |   |   |   |   |   |   |   |   +- categories.json -- 
|   |   |   |   |   |   |   |   |   |   +- categories.wxml -- 
|   |   |   |   |   |   |   |   |   |   +- categories.wxss -- 
|   |   |   |   |   |   |   |   |   +- homeItem -- 
|   |   |   |   |   |   |   |   |   |   +- homeItem.js -- 
|   |   |   |   |   |   |   |   |   |   +- homeItem.json -- 
|   |   |   |   |   |   |   |   |   |   +- homeItem.wxml -- 
|   |   |   |   |   |   |   |   |   |   +- homeItem.wxss -- 
|   |   |   |   |   |   |   |   |   +- index -- 
|   |   |   |   |   |   |   |   |   |   +- index.js -- 
|   |   |   |   |   |   |   |   |   |   +- index.json -- 
|   |   |   |   |   |   |   |   |   |   +- index.wxml -- 
|   |   |   |   |   |   |   |   |   |   +- index.wxss -- 
|   |   |   |   |   |   |   |   |   +- login -- 
|   |   |   |   |   |   |   |   |   |   +- login.js -- 
|   |   |   |   |   |   |   |   |   |   +- login.json -- 
|   |   |   |   |   |   |   |   |   |   +- login.wxml -- 
|   |   |   |   |   |   |   |   |   |   +- login.wxss -- 
|   |   |   |   |   |   |   |   |   +- my -- 
|   |   |   |   |   |   |   |   |   |   +- my.js -- 
|   |   |   |   |   |   |   |   |   |   +- my.json -- 
|   |   |   |   |   |   |   |   |   |   +- my.wxml -- 
|   |   |   |   |   |   |   |   |   |   +- my.wxss -- 
|   |   |   |   |   |   |   |   +- pagesLocation -- 
|   |   |   |   |   |   |   |   |   +- choosePickUpLocation -- 
|   |   |   |   |   |   |   |   |   |   +- choosePickUpLocation.js -- 
|   |   |   |   |   |   |   |   |   |   +- choosePickUpLocation.json -- 
|   |   |   |   |   |   |   |   |   |   +- choosePickUpLocation.wxml -- 
|   |   |   |   |   |   |   |   |   |   +- choosePickUpLocation.wxss -- 
|   |   |   |   |   |   |   |   |   +- myPickUpLocation -- 
|   |   |   |   |   |   |   |   |   |   +- myPickUpLocation.js -- 
|   |   |   |   |   |   |   |   |   |   +- myPickUpLocation.json -- 
|   |   |   |   |   |   |   |   |   |   +- myPickUpLocation.wxml -- 
|   |   |   |   |   |   |   |   |   |   +- myPickUpLocation.wxss -- 
|   |   |   |   |   |   |   |   +- pagesOrder -- 
|   |   |   |   |   |   |   |   |   +- confirmOrder -- 
|   |   |   |   |   |   |   |   |   |   +- confirmOrder.js -- 
|   |   |   |   |   |   |   |   |   |   +- confirmOrder.json -- 
|   |   |   |   |   |   |   |   |   |   +- confirmOrder.wxml -- 
|   |   |   |   |   |   |   |   |   |   +- confirmOrder.wxss -- 
|   |   |   |   |   |   |   |   |   +- getOrderInfo -- 
|   |   |   |   |   |   |   |   |   |   +- getOrderInfo.js -- 
|   |   |   |   |   |   |   |   |   |   +- getOrderInfo.json -- 
|   |   |   |   |   |   |   |   |   |   +- getOrderInfo.wxml -- 
|   |   |   |   |   |   |   |   |   |   +- getOrderInfo.wxss -- 
|   |   |   |   |   |   |   |   |   +- orderList -- 
|   |   |   |   |   |   |   |   |   |   +- orderList.js -- 
|   |   |   |   |   |   |   |   |   |   +- orderList.json -- 
|   |   |   |   |   |   |   |   |   |   +- orderList.wxml -- 
|   |   |   |   |   |   |   |   |   |   +- orderList.wxss -- 
|   |   |   |   |   |   |   |   +- pagesSeckill -- 
|   |   |   |   |   |   |   |   |   +- seckill -- 
|   |   |   |   |   |   |   |   |   |   +- seckill.js -- 
|   |   |   |   |   |   |   |   |   |   +- seckill.json -- 
|   |   |   |   |   |   |   |   |   |   +- seckill.wxml -- 
|   |   |   |   |   |   |   |   |   |   +- seckill.wxss -- 
|   |   |   |   |   |   |   |   +- project.config.json -- 
|   |   |   |   |   |   |   |   +- project.private.config.json -- 
|   |   |   |   |   |   |   |   +- static -- 
|   |   |   |   |   |   |   |   |   +- images -- 
|   |   |   |   |   |   |   |   |   +- logo.png -- 
|   |   |   |   +- yarn.lock -- 
|   |   +- 06-guigu-ssyx-parent -- 
|   |   |   +- .idea -- 
|   |   |   +- common -- 
|   |   |   |   +- common-util -- 
|   |   |   |   |   +- pom.xml -- 
|   |   |   |   |   +- src -- 
|   |   |   |   |   |   +- main -- 
|   |   |   |   |   |   |   +- java -- 
|   |   |   |   |   |   |   |   +- com -- 
|   |   |   |   |   |   |   |   |   +- atguigu -- 
|   |   |   |   |   |   |   |   |   |   +- ssyx -- 
|   |   |   |   |   |   |   |   |   |   |   +- common -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- utils -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   +- DateUtil.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   +- JwtHelper.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   +- MD5.java -- 
|   |   |   |   |   |   |   +- resources -- 
|   |   |   |   |   |   +- test -- 
|   |   |   |   |   |   |   +- java -- 
|   |   |   |   +- pom.xml -- 
|   |   |   |   +- rabbit_util -- 
|   |   |   |   |   +- pom.xml -- 
|   |   |   |   |   +- src -- 
|   |   |   |   |   |   +- main -- 
|   |   |   |   |   |   |   +- java -- 
|   |   |   |   |   |   |   |   +- com -- 
|   |   |   |   |   |   |   |   |   +- atguigu -- 
|   |   |   |   |   |   |   |   |   |   +- ssyx -- 
|   |   |   |   |   |   |   |   |   |   |   +- mq -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- config -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   +- MQConfig.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   +- MQProducerAckConfig.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- constant -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   +- MqConst.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- service -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   +- RabbitService.java -- 
|   |   |   |   |   |   |   +- resources -- 
|   |   |   |   |   |   +- test -- 
|   |   |   |   |   |   |   +- java -- 
|   |   |   |   +- service-util -- 
|   |   |   |   |   +- pom.xml -- 
|   |   |   |   |   +- src -- 
|   |   |   |   |   |   +- main -- 
|   |   |   |   |   |   |   +- java -- 
|   |   |   |   |   |   |   |   +- com -- 
|   |   |   |   |   |   |   |   |   +- atguigu -- 
|   |   |   |   |   |   |   |   |   |   +- ssyx -- 
|   |   |   |   |   |   |   |   |   |   |   +- common -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- auth -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   +- AuthContextHolder.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   +- LoginMvcConfigurerAdapter.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   +- UserLoginInterceptor.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- config -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   +- MybatisPlusConfig.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   +- RedisConfig.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   +- RedissonConfig.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   +- Swagger2Config.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- constant -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   +- RedisConst.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- exception -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   +- GlobalExceptionHandler.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   +- SsyxException.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- result -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   +- Result.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   +- ResultCodeEnum.java -- 
|   |   |   |   |   |   |   +- resources -- 
|   |   |   |   |   |   +- test -- 
|   |   |   |   |   |   |   +- java -- 
|   |   |   |   |   |   |   |   +- com -- 
|   |   |   |   |   |   |   |   |   +- atguigu -- 
|   |   |   |   |   |   |   |   |   |   +- ssyx -- 
|   |   |   |   |   |   |   |   |   |   |   +- CodeGet.java -- 
|   |   |   +- model -- 
|   |   |   |   +- pom.xml -- 
|   |   |   |   +- src -- 
|   |   |   |   |   +- main -- 
|   |   |   |   |   |   +- java -- 
|   |   |   |   |   |   |   +- com -- 
|   |   |   |   |   |   |   |   +- atguigu -- 
|   |   |   |   |   |   |   |   |   +- ssyx -- 
|   |   |   |   |   |   |   |   |   |   +- enums -- 
|   |   |   |   |   |   |   |   |   |   |   +- ActivityType.java -- 
|   |   |   |   |   |   |   |   |   |   |   +- BillType.java -- 
|   |   |   |   |   |   |   |   |   |   |   +- CouponRangeType.java -- 
|   |   |   |   |   |   |   |   |   |   |   +- CouponStatus.java -- 
|   |   |   |   |   |   |   |   |   |   |   +- CouponType.java -- 
|   |   |   |   |   |   |   |   |   |   |   +- OrderStatus.java -- 
|   |   |   |   |   |   |   |   |   |   |   +- PaymentStatus.java -- 
|   |   |   |   |   |   |   |   |   |   |   +- PaymentType.java -- 
|   |   |   |   |   |   |   |   |   |   |   +- ProcessStatus.java -- 
|   |   |   |   |   |   |   |   |   |   |   +- SkuType.java -- 
|   |   |   |   |   |   |   |   |   |   |   +- user -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- Driver.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- Leader.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- LeaderAccount.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- LeaderBank.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- LeaderBill.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- LeaderUser.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- LeaderWithdraw.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- User.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- UserDelivery.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- UserLoginLog.java -- 
|   |   |   |   |   |   |   |   |   |   |   +- UserType.java -- 
|   |   |   |   |   |   |   |   |   |   +- model -- 
|   |   |   |   |   |   |   |   |   |   |   +- acl -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- Admin.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- AdminRole.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- Permission.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- Role.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- RolePermission.java -- 
|   |   |   |   |   |   |   |   |   |   |   +- activity -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- ActivityInfo.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- ActivityRule.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- ActivitySku.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- CouponInfo.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- CouponRange.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- CouponUse.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- Seckill.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- SeckillSku.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- SeckillSkuNotice.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- SeckillTime.java -- 
|   |   |   |   |   |   |   |   |   |   |   +- base -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- BaseEntity.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- BaseMongoEntity.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- MqRepeatRecord.java -- 
|   |   |   |   |   |   |   |   |   |   |   +- order -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- CartInfo.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- OrderDeliver.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- OrderInfo.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- OrderItem.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- OrderLog.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- OrderReturnApply.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- OrderReturnReason.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- OrderSet.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- PaymentInfo.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- RefundInfo.java -- 
|   |   |   |   |   |   |   |   |   |   |   +- product -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- Attr.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- AttrGroup.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- Category.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- Comment.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- CommentReplay.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- SkuAttrValue.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- SkuImage.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- SkuInfo.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- SkuPoster.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- SkuStockHistory.java -- 
|   |   |   |   |   |   |   |   |   |   |   +- search -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- LeaderEs.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- SkuEs.java -- 
|   |   |   |   |   |   |   |   |   |   |   +- sys -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- Region.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- RegionWare.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- Ware.java -- 
|   |   |   |   |   |   |   |   |   |   +- vo -- 
|   |   |   |   |   |   |   |   |   |   |   +- acl -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- AdminLoginVo.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- AdminQueryVo.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- RoleQueryVo.java -- 
|   |   |   |   |   |   |   |   |   |   |   +- activity -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- ActivityRuleVo.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- CouponRuleVo.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- SeckillQueryVo.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- SeckillSkuNoticeVo.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- SeckillSkuQueryVo.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- SeckillSkuVo.java -- 
|   |   |   |   |   |   |   |   |   |   |   +- order -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- CartInfoVo.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- OrderConfirmVo.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- OrderDeliverVo.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- OrderItemMqVo.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- OrderItemParamVo.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- OrderMqVo.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- OrderQueryVo.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- OrderSubmitVo.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- OrderUserQueryVo.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- StockStatisticsVo.java -- 
|   |   |   |   |   |   |   |   |   |   |   +- product -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- AttrGroupQueryVo.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- CategoryQueryVo.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- CategoryVo.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- SkuInfoQueryVo.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- SkuInfoVo.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- SkuStockLockVo.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- SkuStockVo.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- WareQueryVo.java -- 
|   |   |   |   |   |   |   |   |   |   |   +- search -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- LeaderEsQueryVo.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- SkuEsQueryVo.java -- 
|   |   |   |   |   |   |   |   |   |   |   +- sys -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- RegionVo.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- RegionWareQueryVo.java -- 
|   |   |   |   |   |   |   |   |   |   |   +- user -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- LeaderAddressVo.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- LeaderBillQueryVo.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- LeaderQueryVo.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- LeaderVo.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- UserLoginVo.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- UserQueryVo.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- WeixinVo.java -- 
|   |   |   |   |   |   +- resources -- 
|   |   |   |   |   +- test -- 
|   |   |   |   |   |   +- java -- 
|   |   |   +- pom.xml -- 
|   |   |   +- service -- 
|   |   |   |   +- pom.xml -- 
|   |   |   |   +- service-acl -- 
|   |   |   |   |   +- pom.xml -- 
|   |   |   |   |   +- src -- 
|   |   |   |   |   |   +- main -- 
|   |   |   |   |   |   |   +- java -- 
|   |   |   |   |   |   |   |   +- com -- 
|   |   |   |   |   |   |   |   |   +- atguigu -- 
|   |   |   |   |   |   |   |   |   |   +- ssyx -- 
|   |   |   |   |   |   |   |   |   |   |   +- acl -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- controller -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   +- AdminControlller.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   +- IndexController.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   +- PermissionController.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   +- RoleController.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- mapper -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   +- AdminMapper.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   +- AdminRoleMapper.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   +- PermissionMapper.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   +- RoleMapper.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- service -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   +- AdminRoleService.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   +- AdminService.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   +- impl -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   |   +- AdminRoleServiceImpl.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   |   +- AdminServiceImpl.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   |   +- PermissionServiceImpl.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   |   +- RoleServiceImpl.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   +- PermissionService.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   +- RoleService.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- utils -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   +- PermissionHelper.java -- 
|   |   |   |   |   |   |   |   |   |   |   +- ServiceAclApplication.java -- 
|   |   |   |   |   |   |   +- resources -- 
|   |   |   |   |   |   +- test -- 
|   |   |   |   |   |   |   +- java -- 
|   |   |   |   +- service-activity -- 
|   |   |   |   |   +- pom.xml -- 
|   |   |   |   |   +- src -- 
|   |   |   |   |   |   +- main -- 
|   |   |   |   |   |   |   +- java -- 
|   |   |   |   |   |   |   |   +- com -- 
|   |   |   |   |   |   |   |   |   +- atguigu -- 
|   |   |   |   |   |   |   |   |   |   +- ssyx -- 
|   |   |   |   |   |   |   |   |   |   |   +- activity -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- api -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   +- ActivityInfoApiController.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- controller -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   +- ActivityInfoController.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   +- CouponInfoController.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- mapper -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   +- ActivityInfoMapper.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   +- ActivityRuleMapper.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   +- ActivitySkuMapper.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   +- CouponInfoMapper.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   +- CouponRangeMapper.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   +- CouponUseMapper.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   +- xml -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   |   +- ActivityRuleMapper.xml -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   |   +- ActivitySkuMapper.xml -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   |   +- CouponInfoMapper.xml -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   |   +- CouponRangeMapper.xml -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   |   +- CouponUseMapper.xml -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- service -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   +- ActivityInfoService.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   +- CouponInfoService.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   +- impl -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   |   +- ActivityInfoServiceImpl.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   |   +- CouponInfoServiceImpl.java -- 
|   |   |   |   |   |   |   |   |   |   |   +- ServiceActivityApplication.java -- 
|   |   |   |   |   |   |   +- resources -- 
|   |   |   |   |   |   +- test -- 
|   |   |   |   |   |   |   +- java -- 
|   |   |   |   +- service-cart -- 
|   |   |   |   |   +- pom.xml -- 
|   |   |   |   |   +- src -- 
|   |   |   |   |   |   +- main -- 
|   |   |   |   |   |   |   +- java -- 
|   |   |   |   |   |   |   |   +- com -- 
|   |   |   |   |   |   |   |   |   +- atguigu -- 
|   |   |   |   |   |   |   |   |   |   +- ssyx -- 
|   |   |   |   |   |   |   |   |   |   |   +- cart -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- controller -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   +- CartApiController.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- receiver -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   +- CartReceiver.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- service -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   +- CartInfoService.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   +- impl -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   |   +- CartInfoServiceImpl.java -- 
|   |   |   |   |   |   |   |   |   |   |   +- ServiceCartApplication.java -- 
|   |   |   |   |   |   |   +- resources -- 
|   |   |   |   |   |   +- test -- 
|   |   |   |   |   |   |   +- java -- 
|   |   |   |   |   |   |   |   +- com -- 
|   |   |   |   |   |   |   |   |   +- atguigu -- 
|   |   |   |   |   |   |   |   |   |   +- test -- 
|   |   |   |   |   |   |   |   |   |   |   +- Demo1.java -- 
|   |   |   |   +- service-home -- 
|   |   |   |   |   +- pom.xml -- 
|   |   |   |   |   +- src -- 
|   |   |   |   |   |   +- main -- 
|   |   |   |   |   |   |   +- java -- 
|   |   |   |   |   |   |   |   +- com -- 
|   |   |   |   |   |   |   |   |   +- atguigu -- 
|   |   |   |   |   |   |   |   |   |   +- ssyx -- 
|   |   |   |   |   |   |   |   |   |   |   +- home -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- config -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   +- ThreadPoolConfig.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- controller -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   +- CategoryApiController.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   +- HomeApiController.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   +- ItemApiController.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- service -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   +- HomeService.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   +- impl -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   |   +- HomeServiceImpl.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   |   +- ItemServiceImpl.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   +- ItemService.java -- 
|   |   |   |   |   |   |   |   |   |   |   +- ServiceHomeApplication.java -- 
|   |   |   |   |   |   |   +- resources -- 
|   |   |   |   |   |   +- test -- 
|   |   |   |   |   |   |   +- java -- 
|   |   |   |   |   |   |   |   +- com -- 
|   |   |   |   |   |   |   |   |   +- atguigu -- 
|   |   |   |   |   |   |   |   |   |   +- ssyx -- 
|   |   |   |   |   |   |   |   |   |   |   +- CompletableFutureDemo1.java -- 
|   |   |   |   |   |   |   |   |   |   |   +- CompletableFutureDemo2.java -- 
|   |   |   |   |   |   |   |   |   |   |   +- CompletableFutureDemo3.java -- 
|   |   |   |   |   |   |   |   |   |   |   +- CompletableFutureDemo4.java -- 
|   |   |   |   |   |   |   |   |   |   |   +- CompletableFutureDemo5.java -- 
|   |   |   |   +- service-order -- 
|   |   |   |   |   +- pom.xml -- 
|   |   |   |   |   +- src -- 
|   |   |   |   |   |   +- main -- 
|   |   |   |   |   |   |   +- java -- 
|   |   |   |   |   |   |   |   +- com -- 
|   |   |   |   |   |   |   |   |   +- atguigu -- 
|   |   |   |   |   |   |   |   |   |   +- ssyx -- 
|   |   |   |   |   |   |   |   |   |   |   +- order -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- controller -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   +- OrderInfoController.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- mapper -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   +- OrderInfoMapper.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   +- OrderItemMapper.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   +- xml -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   |   +- OrderInfoMapper.xml -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   |   +- OrderItemMapper.xml -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- receiver -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   +- OrderReceiver.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- service -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   +- impl -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   |   +- OrderInfoServiceImpl.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   +- OrderInfoService.java -- 
|   |   |   |   |   |   |   |   |   |   |   +- ServiceOrderApplication.java -- 
|   |   |   |   |   |   |   +- resources -- 
|   |   |   |   |   |   +- test -- 
|   |   |   |   |   |   |   +- java -- 
|   |   |   |   +- service-payment -- 
|   |   |   |   |   +- pom.xml -- 
|   |   |   |   |   +- src -- 
|   |   |   |   |   |   +- main -- 
|   |   |   |   |   |   |   +- java -- 
|   |   |   |   |   |   |   |   +- com -- 
|   |   |   |   |   |   |   |   |   +- atguigu -- 
|   |   |   |   |   |   |   |   |   |   +- ssyx -- 
|   |   |   |   |   |   |   |   |   |   |   +- payment -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- controller -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   +- WeixinController.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- mapper -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   +- PaymentInfoMappper.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- service -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   +- impl -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   |   +- PaymentInfoServiceImpl.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   |   +- WeixinServiceImpl.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   +- PaymentInfoService.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   +- WeixinService.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- utils -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   +- ConstantPropertiesUtils.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   +- HttpClient.java -- 
|   |   |   |   |   |   |   |   |   |   |   +- ServicePaymentApplication.java -- 
|   |   |   |   |   |   |   +- resources -- 
|   |   |   |   |   |   +- test -- 
|   |   |   |   |   |   |   +- java -- 
|   |   |   |   +- service-product -- 
|   |   |   |   |   +- pom.xml -- 
|   |   |   |   |   +- src -- 
|   |   |   |   |   |   +- main -- 
|   |   |   |   |   |   |   +- java -- 
|   |   |   |   |   |   |   |   +- com -- 
|   |   |   |   |   |   |   |   |   +- atguigu -- 
|   |   |   |   |   |   |   |   |   |   +- ssyx -- 
|   |   |   |   |   |   |   |   |   |   |   +- product -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- api -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   +- ProductInnnerController.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- controller -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   +- AttrController.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   +- AttrGroupController.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   +- CategoryController.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   +- FileUploadController.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   +- SkuInfoController.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- mapper -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   +- AttrGroupMapper.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   +- AttrMapper.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   +- CategoryMapper.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   +- SkuAttrValueMapper.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   +- SkuImageMapper.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   +- SkuInfoMapper.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   +- SkuPosterMapper.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   +- xml -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   |   +- AttrGroupMapper.xml -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   |   +- AttrMapper.xml -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   |   +- CategoryMapper.xml -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   |   +- SkuAttrValueMapper.xml -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   |   +- SkuImageMapper.xml -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   |   +- SkuInfoMapper.xml -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   |   +- SkuPosterMapper.xml -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- receiver -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   +- StockReceiver.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- service -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   +- AttrGroupService.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   +- AttrService.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   +- CategoryService.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   +- FileUploadService.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   +- impl -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   |   +- AttrGroupServiceImpl.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   |   +- AttrServiceImpl.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   |   +- CategoryServiceImpl.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   |   +- FileUploadServiceImpl.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   |   +- SkuAttrValueServiceImpl.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   |   +- SkuImageServiceImpl.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   |   +- SkuInfoServiceImpl.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   |   +- SkuPosterServiceImpl.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   +- SkuAttrValueService.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   +- SkuImageService.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   +- SkuInfoService.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   +- SkuPosterService.java -- 
|   |   |   |   |   |   |   |   |   |   |   +- ServiceProductApplication.java -- 
|   |   |   |   |   |   |   +- resources -- 
|   |   |   |   |   |   +- test -- 
|   |   |   |   |   |   |   +- java -- 
|   |   |   |   +- service-search -- 
|   |   |   |   |   +- pom.xml -- 
|   |   |   |   |   +- src -- 
|   |   |   |   |   |   +- main -- 
|   |   |   |   |   |   |   +- java -- 
|   |   |   |   |   |   |   |   +- com -- 
|   |   |   |   |   |   |   |   |   +- atguigu -- 
|   |   |   |   |   |   |   |   |   |   +- ssyx -- 
|   |   |   |   |   |   |   |   |   |   |   +- search -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- controller -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   +- SkuApiController.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- receiver -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   +- SkuReceiver.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- repository -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   +- SkuRepository.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- service -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   +- impl -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   |   +- SkuServiceImpl.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   +- SkuService.java -- 
|   |   |   |   |   |   |   |   |   |   |   +- ServiceSearchApplication.java -- 
|   |   |   |   |   |   |   +- resources -- 
|   |   |   |   |   |   +- test -- 
|   |   |   |   |   |   |   +- java -- 
|   |   |   |   +- service-sys -- 
|   |   |   |   |   +- pom.xml -- 
|   |   |   |   |   +- src -- 
|   |   |   |   |   |   +- main -- 
|   |   |   |   |   |   |   +- java -- 
|   |   |   |   |   |   |   |   +- com -- 
|   |   |   |   |   |   |   |   |   +- atguigu -- 
|   |   |   |   |   |   |   |   |   |   +- ssyx -- 
|   |   |   |   |   |   |   |   |   |   |   +- ServiceSysApplication.java -- 
|   |   |   |   |   |   |   |   |   |   |   +- sys -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- controller -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   +- RegionController.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   +- RegionWareController.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   +- WareController.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- mapper -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   +- RegionMapper.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   +- RegionWareMapper.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   +- WareMapper.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   +- xml -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   |   +- RegionMapper.xml -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   |   +- RegionWareMapper.xml -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   |   +- WareMapper.xml -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- service -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   +- impl -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   |   +- RegionServiceImpl.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   |   +- RegionWareServiceImpl.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   |   +- WareServiceImpl.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   +- RegionService.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   +- RegionWareService.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   +- WareService.java -- 
|   |   |   |   |   |   |   +- resources -- 
|   |   |   |   |   |   +- test -- 
|   |   |   |   |   |   |   +- java -- 
|   |   |   |   +- service-user -- 
|   |   |   |   |   +- pom.xml -- 
|   |   |   |   |   +- src -- 
|   |   |   |   |   |   +- main -- 
|   |   |   |   |   |   |   +- java -- 
|   |   |   |   |   |   |   |   +- com -- 
|   |   |   |   |   |   |   |   |   +- atguigu -- 
|   |   |   |   |   |   |   |   |   |   +- ssyx -- 
|   |   |   |   |   |   |   |   |   |   |   +- ServiceUserApplication.java -- 
|   |   |   |   |   |   |   |   |   |   |   +- user -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- api -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   +- LeaderAddressApiController.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- controller -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   +- WeixinApiController.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- mapper -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   +- LeaderMapper.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   +- UserDeliveryMapper.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   +- UserMapper.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- service -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   +- impl -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   |   +- UserServiceImpl.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   +- UserService.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- utils -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   +- ConstantPropertiesUtil.java -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   +- HttpClientUtils.java -- 
|   |   |   |   |   |   |   +- resources -- 
|   |   |   |   |   |   +- test -- 
|   |   |   |   |   |   |   +- java -- 
|   |   |   +- service-client -- 
|   |   |   |   +- pom.xml -- 
|   |   |   |   +- service-activity-client -- 
|   |   |   |   |   +- pom.xml -- 
|   |   |   |   |   +- src -- 
|   |   |   |   |   |   +- main -- 
|   |   |   |   |   |   |   +- java -- 
|   |   |   |   |   |   |   |   +- com -- 
|   |   |   |   |   |   |   |   |   +- atguigu -- 
|   |   |   |   |   |   |   |   |   |   +- ssyx -- 
|   |   |   |   |   |   |   |   |   |   |   +- activity -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- client -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   +- ActivityFeignClient.java -- 
|   |   |   |   |   |   |   +- resources -- 
|   |   |   |   |   |   +- test -- 
|   |   |   |   |   |   |   +- java -- 
|   |   |   |   +- service-cart-client -- 
|   |   |   |   |   +- pom.xml -- 
|   |   |   |   |   +- src -- 
|   |   |   |   |   |   +- main -- 
|   |   |   |   |   |   |   +- java -- 
|   |   |   |   |   |   |   |   +- com -- 
|   |   |   |   |   |   |   |   |   +- atguigu -- 
|   |   |   |   |   |   |   |   |   |   +- ssyx -- 
|   |   |   |   |   |   |   |   |   |   |   +- cart -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- client -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   +- CartFeignClient.java -- 
|   |   |   |   |   |   |   +- resources -- 
|   |   |   |   |   |   +- test -- 
|   |   |   |   |   |   |   +- java -- 
|   |   |   |   +- service-order-client -- 
|   |   |   |   |   +- pom.xml -- 
|   |   |   |   |   +- src -- 
|   |   |   |   |   |   +- main -- 
|   |   |   |   |   |   |   +- java -- 
|   |   |   |   |   |   |   |   +- com -- 
|   |   |   |   |   |   |   |   |   +- atguigu -- 
|   |   |   |   |   |   |   |   |   |   +- ssyx -- 
|   |   |   |   |   |   |   |   |   |   |   +- order -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- client -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   +- OrderFeignClient.java -- 
|   |   |   |   |   |   |   +- resources -- 
|   |   |   |   |   |   +- test -- 
|   |   |   |   |   |   |   +- java -- 
|   |   |   |   +- service-product-client -- 
|   |   |   |   |   +- pom.xml -- 
|   |   |   |   |   +- src -- 
|   |   |   |   |   |   +- main -- 
|   |   |   |   |   |   |   +- java -- 
|   |   |   |   |   |   |   |   +- com -- 
|   |   |   |   |   |   |   |   |   +- atguigu -- 
|   |   |   |   |   |   |   |   |   |   +- ssyx -- 
|   |   |   |   |   |   |   |   |   |   |   +- client -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- product -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   +- ProductFeignClient.java -- 
|   |   |   |   |   |   |   +- resources -- 
|   |   |   |   |   |   +- test -- 
|   |   |   |   |   |   |   +- java -- 
|   |   |   |   +- service-search-client -- 
|   |   |   |   |   +- pom.xml -- 
|   |   |   |   |   +- src -- 
|   |   |   |   |   |   +- main -- 
|   |   |   |   |   |   |   +- java -- 
|   |   |   |   |   |   |   |   +- com -- 
|   |   |   |   |   |   |   |   |   +- atguigu -- 
|   |   |   |   |   |   |   |   |   |   +- ssyx -- 
|   |   |   |   |   |   |   |   |   |   |   +- client -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- search -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   +- SkuFeignClient.java -- 
|   |   |   |   |   |   |   +- resources -- 
|   |   |   |   |   |   +- test -- 
|   |   |   |   |   |   |   +- java -- 
|   |   |   |   +- service-user-client -- 
|   |   |   |   |   +- pom.xml -- 
|   |   |   |   |   +- src -- 
|   |   |   |   |   |   +- main -- 
|   |   |   |   |   |   |   +- java -- 
|   |   |   |   |   |   |   |   +- com -- 
|   |   |   |   |   |   |   |   |   +- atguigu -- 
|   |   |   |   |   |   |   |   |   |   +- ssyx -- 
|   |   |   |   |   |   |   |   |   |   |   +- client -- 
|   |   |   |   |   |   |   |   |   |   |   |   +- user -- 
|   |   |   |   |   |   |   |   |   |   |   |   |   +- UserFeignClient.java -- 
|   |   |   |   |   |   |   +- resources -- 
|   |   |   |   |   |   +- test -- 
|   |   |   |   |   |   |   +- java -- 
|   |   |   +- service-gateway -- 
|   |   |   |   +- pom.xml -- 
|   |   |   |   +- src -- 
|   |   |   |   |   +- main -- 
|   |   |   |   |   |   +- java -- 
|   |   |   |   |   |   |   +- com -- 
|   |   |   |   |   |   |   |   +- atguigu -- 
|   |   |   |   |   |   |   |   |   +- ssyx -- 
|   |   |   |   |   |   |   |   |   |   +- config -- 
|   |   |   |   |   |   |   |   |   |   |   +- CorsConfig.java -- 
|   |   |   |   |   |   |   |   |   |   +- ServiceGatewayApplication.java -- 
|   |   |   |   |   |   +- resources -- 
|   |   |   |   |   +- test -- 
|   |   |   |   |   |   +- java -- 
|   |   +- sql -- 
|   |   |   +- 数据库.sql -- 
|   +- 尚上优选.txt -- 
|   +- 画图 -- 
|   +- 课件 -- 
|   |   +- 尚上优选课件v1.1 -- 
|   |   |   +- images -- 
|   |   |   +- 企业级微服务架构项目-尚上优选项目.md -- 
```

#### 后端技术栈

| 技术                             | 版本            | 说明                          |
|--------------------------------|---------------|-----------------------------|
| 示例: Spring Boot Starter Parent | 2.0.4.RELEASE | Spring Boot 父依赖             |

#### 前端技术栈

| 技术       | 版本         | 说明                                       |
|----------|------------|------------------------------------------|
| 示例：axios | ^0.16.2    | HTTP请求库                                  |


#### 安装教程


#### 登录账户

#### 截图

#### 拓展知识
