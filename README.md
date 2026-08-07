# luopan(罗盘)

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Version](https://img.shields.io/github/v/tag/saudademjj/luopan?label=version)](https://github.com/saudademjj/luopan)
[![Rules](https://img.shields.io/badge/rules-16-blue)](skills/travel-planner/SKILL.md)
[![Tested: 6 cities](https://img.shields.io/badge/tested-6%20cities-brightgreen)](ITERATIONS.md)
[![Docs](https://img.shields.io/badge/docs-online-8A2BE2)](https://saudade.me/luopan/)

一款旅游行程规划 skill。排程规则按 16 条整理(R1-R13 加 3 条红线),每条都来自一次真实的反馈:先排一版行程,再请熟悉当地的人挑错,把错处写回规则。试过的城市:南京(3 轮)、苏州、杭州、北京(2 轮)、伊犁自驾(2 轮)。

## 特性

- 预算没确认前,只输出问题清单,不出行程草稿
- 行程范围等于指定的目的地,不擅自加周边城市。区域环线跨出指定范围时说明原因,并给出严格版替代
- 票价、开放时间等事实性数据优先官方渠道,自媒体和野榜只作线索,标注"需官方确认";每条数据带来源和查询日期
- 浏览时间之外留出排队、交通、吃饭、拍照的余量;顶流园区独占一天;自驾单日车程计入体量
- 交付前重读规则,逐条填自检表(带证据)。长行程里规则容易走样,这一步是兜底
- 输出包含:逐日行程表、预算估算(经济/舒适两档)、交通住宿建议、景点和美食清单(含避雷)、二次确认清单、数据来源索引

## 安装

### 方式一:插件安装

在支持插件系统的客户端终端里执行两步:

```bash
plugin marketplace add saudademjj/luopan
plugin install travel-planner
```

本地调试可以用本地路径:`plugin marketplace add /path/to/luopan`,然后 `plugin install travel-planner`。

### 方式二:手动复制

把 `skills/travel-planner` 整个目录复制到你的技能(skills)目录。

## 使用

直接提旅行需求,skill 会自动触发:

> "帮我规划去苏州 5 天,带爸妈"
> "北京 7 天 6 晚,情侣,预算中等"
> "伊犁自驾 9 天,5 人,从乌鲁木齐出发"

第一步先收集需求(预算必问),确认后才联网调研、排行程。也可以显式调用。

## 规则怎么来的

| 规则 | 来源反馈 |
|---|---|
| 范围 | "我只说了南京游,为什么要安排扬州镇江" |
| 优先级分级 | "牛首山到底排前百分之多少,台城不是热门景点" |
| 顶流园区独占一天 | "红山动物园最起码得一天,得到晚上" |
| 时间缓冲 | "估算浏览时间再加 1-2 小时,要排队、交通、吃饭、拍照" |
| 高商业化旅游街避雷 | "山塘街这种商业化非常严重的地方,吃的全国统一" |
| 全局去重 | "晚上去了两次双塔市集+山塘街" |
| 主观体验类可选化 | "印象西湖、游船这种要让游客决定要不要" |
| 来源分级 | "搜狐美食榜是野榜,自媒体不能全信" |

完整的迭代记录见 [ITERATIONS.md](ITERATIONS.md)。

## 数据时效

行程里的票价、开放时间、通行政策都带查询日期,输出末尾有"出行前二次确认清单",出发前请核对官方渠道。

## 示例输出

- [伊犁 10 天自驾环线(含独库公路北段)](examples/ili-10day-itinerary.md),含规则自检表、数据来源索引

## License

[MIT](LICENSE)
