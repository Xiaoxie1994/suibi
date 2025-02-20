---
icon: en-to-square
date: 2024-10-12
category:
  - AI探索
  - 技术提效
tag:
  - AI
  - 智能体
  - 技术调研
---

# 我的内容创作最强搭子——Kimi
如果说编程上有难题，现在第一个想到的是问GPT，一般能给出比较满意的答案，生成的代码也基本靠谱。

但由于网络和中文语境要求，日常还是更多使用国内的大模型。在众多国内大模型中，笔者为何对Kimi情有独钟呢？因为我收...那必须是因为它的强项——**长文本解读能力**啦！

<!-- more -->

![](https://fastly.jsdelivr.net/gh/bucketio/img0@main/2024/10/11/1728653751927-a3043a57-b2d8-4ed0-9fe6-a3dcbc7efa56.png)

## 初识Kimi
初识是在大牛猫的文章里，某期日更里提到了AI独角兽公司“**月之暗面**”和它旗下的产品**Kimi**。当时还是比较初期的版本，大牛猫用它解读了一些文档，都能给出一些比较好的归纳，后面又陆续提到过几次，就记住了。

![](https://fastly.jsdelivr.net/gh/bucketio/img12@main/2024/10/11/1728655092434-0b527764-9059-49b2-94c6-333200d56cd7.png)

恰逢那段时间在整理“代码可视化”的理论知识，会进行大量的检索和文字阅读，十分的耗费精力。随即就想到了Kimi，网站版自带了检索能力，再结合长文本解读能力，着实节省了我不少素材找寻和解读的时间。

## 内容创作v1.0
有了这次不错的体验后，后续使用Kimi的就更频繁了，但也仅仅停留在简单的文本解读上。直到有一天笔者突然问了Kimi这么一个问题（至于为什么问这个问题就不得而知了）：

![](https://fastly.jsdelivr.net/gh/bucketio/img18@main/2024/10/11/1728655679168-66d76ae9-68d6-4dfa-9080-251f21ffd998.png)

回答的第一条是“**知识与学习**”。但学习的方式有很多种，对笔者而言了解新技术和新热点是保持职业热爱很重要的方式。但日常工作已经占用了大量的时间，根本就没有时间搜集并学习新知识。

就想如果有一个工具能**自动抓取技术热点并将长篇大论的文字浓缩为100~200字左右的摘要**，这样每天花半个小时就能消化信息了，这也太棒了吧。

于是做了第一次尝试，实现了一个自动抓取热点并总结的小工具，实现思路见下图。内容回顾戳👉🏻 [没时间了解技术热点？让大模型帮你整理重点吧！](https://mp.weixin.qq.com/s/qelnn3DWsOic0_5iXMKrJw)

![](https://fastly.jsdelivr.net/gh/bucketio/img5@main/2024/10/11/1728656247843-80967bb2-f3be-4149-9f1e-eb577aae7aea.png)

不过这一版工具有一个缺陷，就是当时Kimi的API不支持搜索功能（目前已支持，戳👉🏻[Kimi API 支持联网搜索增强了！](https://mp.weixin.qq.com/s/BWVAAvqnGum3iIg93pJhuA)），于是笔者自己手搓了一个页面检索和内容解析工具，但由于没有处理噪音整体效果比较一般。

但通过这次尝试至少跑通了流程。接着字节推出了coze，也第一时间集成到了工具中。工作流体验确实很不错，替换掉了自己写的搜索和内容解析工具。

![](https://fastly.jsdelivr.net/gh/bucketio/img5@main/2024/10/11/1728657739857-e056914e-c3ae-4b06-8292-4712b204a2bf.png)

再之后的事大家都知道了，笔者开始发**技术周刊**了！

![](https://fastly.jsdelivr.net/gh/bucketio/img3@main/2024/10/11/1728657483200-149807bd-6e85-4998-8b7d-fcc6500ae29c.png)

## 内容创作v2.0
不过在第7期的时候笔者逐渐放弃了这个小工具，转而人工的收集周刊内容。究其原因主要有两点：

### 内容准确度较差
这个准确度不是指Kimi总结的内容和原文的差异，指的是收集的很多文章本身是没有营养的，这主要受限于信息源的质量和笔者手搓的爬虫缺少数据预处理能力。

同时也考虑到既然周刊公开发布了，要对自己的内容负责，至少保证最后选出的内容都阅读过一遍。因此在迭代爬虫和转人工中，选择了后者。

![](https://fastly.jsdelivr.net/gh/bucketio/img14@main/2024/10/11/1728659145536-d20ab013-10cd-4f17-90c5-6c99fba59ccb.png)

### Kimi发布浏览器插件了！
刚好7月Kimi发布了一个超好用的功能“[Kimi 浏览器插件来了！](https://mp.weixin.qq.com/s/-srEcOwDiEoHp1tTdleTPA)”，省去了人工粘贴文章链接到Kimi主页的过程，在原始页面上就能进行内容摘要生成。由于这个功能的出现，转人工处理后工作量也没有较大上涨（要是工作量大也坚持不了多久😂）。

![](https://fastly.jsdelivr.net/gh/bucketio/img5@main/2024/10/11/1728659698339-ac1726cb-6170-4313-ab06-23ca05b920b8.png)

## 内容创作v3.0
现在，Kimi发布了新的重磅功能“[Kimi 探索版来了，最好的搜索是不用自己搜索](https://mp.weixin.qq.com/s/cRXe0HFO5BX0AzziaqoiKg)”，补齐了信息搜索这一拼图，终于能彻底解放双手啦？官方对探索版的定义是：

> Kimi 探索版具备 AI 自主搜索能力，可以模拟人类的推理思考过程，多级分解复杂问题，执行深度搜索，并即时反思改进结果，提供更全面和准确的答案，帮助你更高效地完成分析调研等复杂任务。

![](https://fastly.jsdelivr.net/gh/bucketio/img1@main/2024/10/11/1728660032061-85b50d2c-8d50-4300-b5eb-bca2d6a5217e.png)

看了官方示例，更多是帮助用户**节省花在搜索调研任务上的时间**，让大家可以有更多时间**专注于提出问题、思考和创造**。

![](https://fastly.jsdelivr.net/gh/bucketio/img16@main/2024/10/11/1728660483053-732aa9ed-ddc4-4457-9201-b5114a9b3a57.gif)

咦？这好像和笔者之前用过的一个工具有点相似（相关内容戳👉🏻 [用 AI 解锁技术调研的新姿势](https://mp.weixin.qq.com/s/hzZHwjKH5IE6H0yNXVhDPQ)）。不过虽然都是针对调研场景，STORM主要的检索页面和生成的结果都是英文的，在知识库选择和语境上还是有明显的差异。**Kimi更适合中国宝宝体质！**

![](https://fastly.jsdelivr.net/gh/bucketio/img18@main/2024/10/11/1728660744143-52c8de18-0706-411a-95ef-0af09e3d6777.png)

让Kimi汇总“本周技术人应该关注的热点信息”，得到的结果颇具参考意义。信息有来源可追溯，关键是能节省看网站的时间，想想319个网站全部看一遍标题都得费些功夫了。

![](https://fastly.jsdelivr.net/gh/bucketio/img2@main/2024/10/11/1728661394008-55798098-3850-4b10-adab-fa5e32ffe191.png)

别忘了Kimi还支持**多轮对话**，能够按照诉求对生成内容进行调整，理论上有更强的扩展性。

所以是时候再迭代一下“**热点收集小工具**”了，把这些新特性融入进去，可能就能实现最初的梦想——**坐等AI把饭**（有用的信息）**喂嘴里**。

![](https://fastly.jsdelivr.net/gh/bucketio/img5@main/2024/10/12/1728663283269-f77a2bcf-ee06-4080-8236-2ecfbef62e49.png)

最后也希望Kimi越来越好，能够杀出重围，持续提供更多真正好用的功能。

<div style="text-align: center;"> —— 完 —— </div>

---
关注“**肖恩聊技术**”公众号，原创技术文章第一时间推送~

<img src="https://cdn.jsdelivr.net/gh/Xiaoxie1994/images/images/20241103221454.png" alt="公众号二维码" width="300">