---
title: "使用 Cursor 做了几个单页小工具"
date: 2024-12-21T11:13:43+0800
tags: [折腾]
feature: https://r2.immmmm.com/2024/12/SCR-20241221-nwtm.png.webp
---

最大感受，说清楚需求，基本上第一次对话即可生成。之后都是叠加需求和反复修复的过程。

最大感慨，需求是稀缺资源，真切合理的需求结合 AI，把之前根本不会想尝试，变为积极主动试一试。

<!--more-->

### 由简到难的 24 点出题器

![](https://r2.immmmm.com/2024/12/SCR-20241221-nqww.png.webp)
![](https://r2.immmmm.com/2024/12/SCR-20241221-nqxm.png.webp)

「24 点出题器」 <https://edui123.com/24/>

把 1362 道有解的 24 点题目，依据难度排序，支持按序和随机出题，右上角有 30 秒倒计时，点击标题可查看解法。

玩 24 点日常难受的点在于直接拿扑克牌玩，1820 个不同组合，而实际有解的只有 1362 个。1362/1820≈0.748≈75%，四局有一局无解，已经很打击兴趣咯。

很早看到 [4数网](https://www.4shu.net/game/difficulties/) 经过难度排序的题库，基于世界各地的人们已经解决 6283289 个题目，计算了每道题目的 “统一中值解决时间”, 并从最简单到最难给这些题目排序。

一拍即合，干活！

### 语文生字拼音匹配小游戏

![](https://r2.immmmm.com/2024/12/SCR-20241221-npdd.png.webp)
![](https://r2.immmmm.com/2024/12/SCR-20241221-npiy.png.webp)

「认读小能手」 <https://edui123.com/renzi/>

基于部编语文一年级上册“识字表”中的 280 字，给认读生字增加一点趣味互动性，家里或学校能在期末阶段用上一用。

- 3 种模式可选：限时 1 分钟、3 分钟、不限时；
- 拖动拼音到对应的汉字上方，右上角有实时的统计数据条。
- 限时模型下，结束时会有统计数据汇总，还有过程中拖动错误的汉字记录回顾。

### 自动听写词语

![](https://r2.immmmm.com/2024/12/SCR-20241221-nsoi.png.webp)
![](https://r2.immmmm.com/2024/12/SCR-20241221-nsqr.png.webp)

「词语听写」 <https://edui123.com/tingxie>

一个自动朗读语文书后“词语表”的在线网页。

- 内置 3~6 年级上册词语，选择年级、第几课，点击开始即可；
- 默认每个词语读两遍，不同词语停顿 3 秒（可拖动修改）；
- 随机模式，全册词语打乱顺序 20 个为一组；
- 早读模式，全册词语打乱顺序读完后会显示“词语”。

### 杂记

其实 3 个都是单页可离线的 html，听写后来改用第三方接口，因为发现 Edge 文字转语音国内不可用，能用也只能 PC 上，使用太受限。