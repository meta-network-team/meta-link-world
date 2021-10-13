---
title: 瞬Matataki 4.9.0 版本更新报告
tags: []
updated: '2021-10-12T22:52:46.209Z'
categories: []
excerpt: ''
date: 2021-10-12 22:52:46
---

\[TOC]

# ✨Matataki 4.9.0 版本新功能简报

**版本号：** 4.9.0 版本
**开发周期：** 2020年11月9号~2020年11月30号
**策划人：** 林可、小岛
**开发者：** Frank、Garfield550、小田、LittleSound、Neko、

## 更新内容

**Matataki**
`新增` 可将文章添加到自定义收藏夹功能

`新增`  Bilibili + twitter 混合时间轴

`新增` 在个人主页中默认只展示未下架的内容

`优化` 修复了Metamask无法登入的bug

`优化` 移除了“我的账户”-->“收藏夹”路径

**Fan票**
`新增` 支持Fan票导出到 币安智能链

\==Matataki的平台代币 META 已经内测发行==

<iframe width="100%" height="200px" src='https://www.matataki.io/widget/token/?id=120' frameborder=0></iframe>

# 📑功能详解

下面我将会对上述提到的重点功能进行详细说明

## 📜混合时间轴

在上一期的开发中，我们已经成功引入了个人的Twitter时间轴，不过在那个版本中，需要进入对方Matataki个人主页中去查看时间轴，并不够方便。因此在这一期中，我们带来了增强版本的混合时间轴

### 这是什么

我们希望将 社交媒体（SocialMedia） 与 社交资金（SocialMoney）打通，因此我们的第一步就是聚合社交媒体的信息。现在我们支持用户通过绑定自己的 Twitter 账号 和 Bilibili 账号 来在 瞬Matataki 上同步自己在 社交媒体上的时间轴。而你的关注者们则可以在 瞬Matataki 上像是查看普通动态一样 同步看到你在多个社交平台上的动态信息。从而 实现 多处操作，一处查看，将你的Fan票价值和你的社交价值 进行绑定。

![image.png](ipfs://QmVBKemorD4kvtMDRi8tV1RPZNgxEGbP1CRehDVyzBrbHk)

### 使用规则

**如何查看混合时间轴**
在点击导航栏中的 “动态”-->“第三方时间轴” 即可查看。不过只有你关注的对象已经绑定了Twitter账号 和 Bilibili账号 才可以在“第三方时间轴”中查看到他们的动态。

**如何同步 Bilibili 时间轴**
前往[账号管理](https://matataki.io/setting/account)中，在“Matataki Auth 绑定的账号”中即可看到 Bilibili账号的绑定入口，点击之后根据页面提示进行绑定即可。绑定完成后，系统会自动同步时间轴。

关于Matataki Auth ：这是Matataki的下一代社交聚合验证中心，和主账号不同的是在这里绑定的账号不可用于Matataki登录。

**如何同步 Twitter 时间轴**
进入你的个人主页打开twitter标签页，然后根据引导的步骤即可完成绑定。

1.  绑定Twitter账号（绑定后即可使用twitter直接登录）
2.  授权同步时间线信息
    绑定完成后，系统会自动同步时间轴

注意事项
目前 此功能 还在测试中，可能存在使用上的问题。如果发现了我们的不足或是缺陷，欢迎来[表单反馈](http://andoromeda.mikecrm.com/a93Le8z) 。

## 🌌Fan票跨链导出至 BSC 币安智能链（Fan票折跃门DAPP）

瞬Matataki 是 Fan票 的 MotherLand ，通过折跃门后 Fan票 则可以前往更广阔的 星辰大海 ，在不同的位面穿梭（跨链）。

众所周知，Fan票原生是发行在 以太坊 的 Rinkeby 网络上的。在Defi的浪潮下，Fan票不仅需要在 瞬Matataki游乐场中 使用，还要能够和区块链基础设施接轨。因此将Fan票跨链到以太坊的各种智能链就成为了一项重要的任务。

在众多的链中，我们优先选择了 BSC 币安智能链，因为在这条链上的交易手续费够低，符合社交代币的 大量&小额 的实际应用场景需求。最初我们选择了Rinkeby而不是以太坊主网也是基于同样的考虑。

### 什么是折跃门

这是 瞬Matataki 推出的 Fan票 跨链导入/导出 工具。目前已经整合了 Rinkeby 和 BSC主网 双向导入导出，目前跨链导出之后Fan票的合约地址会改变，需要去交易记录中手动获取跨链后Fan票地址，未来会支持在前端直接展示。

\==Tips 什么是BSC ：这是币安基于以太坊推出的一条智能链，可以直接通过Metamask插件钱包或是Math麦子手机钱包访问。[连接教程](https://docs.binance.org/smart-chain/wallet/metamask.html)==

### 如何使用折跃门

DAPP地址：<https://matataki.io/token/in-n-out> ,或者是在[DAPP](https://matataki.io/dapp)页面中找到 “Fan票折跃门”应用。

#### Fan票合约地址

打开Fan票的详情页后，点击复制按钮即可获取Hash（合约地址）
![image.png](ipfs://QmSNhHAdadziAWQmMP92PCfAhuAktjnRTNA3hA9Bw2HtBu)

#### 导出至Rinkeby

1.  打开 折跃门后，选择提取至Rinkeby
2.  准确 选择“类型”、输入“数量”和提取到“目标钱包地址 后确定

#### 导出至BSC

由于跨链导出的缘故，操作上会稍微复杂些

1.  打开 折跃门后，选择提取至BSC
2.  打开 你的Metamask钱包，并切换到BSC正式网，同时确保钱包里有少量的BNB用于支付手续费
3.  准确 选择“类型”、输入“数量”和提取到“目标钱包地址 后确定。此时系统会下发“跨链转账许可”。
    a. 如果你就是提取的目标钱包，点击左边的按钮即可。
    b. 如果你是要提取到别人的钱包中，则点击右侧按钮复制许可，将许可发送给需要提取Fan票的人。

![image.png](ipfs://QmPBacQHnqt98SpN7LopekJLAPsn4FtoEPB3iQ3S26dBx1)

4.  如果你是 3.a 的操作的话，根据界面引导点击“上传许可”后，在弹出的钱包界面中签名（需支付手续费）即可。

![image.png](ipfs://QmWJ24cHBbfpST4Xa4aaHR1j2DsvWAvwYnmHiheNwUWGCQ)

5.  如果你是 3.b 的操作的话，则让你的朋友进入下图所示的“替别人体现许可”页面，粘贴许可信息后即可自动解析，根据引导点击“上传许可”后，在弹出的钱包界面中签名（需支付手续费）即可。

![image.png](ipfs://QmPeHKg6T8r9BwQwW3ACWPNiMxpWimxKjEJBYpNymxiSuY)

#### 从Rinkeby导入

1.  打开 折跃门后，选择从Rinkeby转入
2.  复制页面中你的托管钱包地址（这是Matataki平台生成的属于你的托管钱包）
3.  使用钱包从Rinkeby向托管钱包地址转账 Fan票(请勿转入非Fan票的代币！无法找回)并复制转账交易的Hash
4.  在 折跃门 中填入转账交易的Hash并确定

#### 从BSC导入

功能仍在准备中

### 导出到BSC上可以交易么

是的，推荐使用 Unisave 交易所（这是由我们团队独立开发的交易所），拥有超低滑点、
交易所地址：<https://app.unisave.exchange/>

## 📚自定义收藏夹

瞬Matataki上产出了数量庞大的优质内容，因此我们升级了收藏夹。现在你可以自己创任意数量且具有权限的收藏夹了，也可以将一篇文章收藏到多个收藏夹中方便归类检索。

![image.png](ipfs://QmXjh5zb9cLd1vsL6tP6n3adHnaHcSU5TsR78zKqYK4q9F)

# 📬想说的话

## 关于SocialMoney

最近看到越来越多的 SocialMoney 领域的创新力量都在崛起，我们很高兴走在一条逐渐被认可和接受的道路上。在过去这段时间中，总共新增了10支Fan票。而在Matataki的平台上总共已经发行了98支Fan票，感谢大家的支持和信任。有特别多的社区小伙伴在给我们的产品线出谋划策，甚至还有自己直接动手在我们的基础上进行二次开发的朋友。非常感谢小伙伴们的支持！

<iframe width="100%" height="180" src='https://www.matataki.io/widget/?id=5779&invite=9&referral=9' frameborder=0></iframe>

我们接下来会将主要精力用在为Fan票搭建更多应用场景。这是一条人迹罕至的道路，在这里的商业模式和应用场景都还不够明确，需要我们这样的先行者去探索和试验。我们的目标是让所有人都可以无忧以及轻松的去使用Fan票，而不仅仅是区块链的原住民的玩具。在新的商业模式和应用场景下，几乎所有的基础设施都需要我们自己搭建，不过亲手去建造理想中的世界也正是我们这帮人的 乐趣所在 。这个赛道还很早期，没有成熟的规则，希望大家一起放轻松，感受其中的乐趣所在。

在 Matataki 上基于 Fan票 产生了无数的创作，但是 Matataki 提供的 Blog 形式不足以支撑社群小伙伴们的各种 观察 和 Idea 沉淀。因此我创建了一个语雀组织 [SocialMoney?研究协会](https://www.yuque.com/socialmoney) ，欢迎收藏或申请加入。

**小作业：** 你关于 Fan票 或是 SocialMoney 有过哪些未曾设想的道路？欢迎在评论区将你的想法告诉我们

## 关于瞬Matataki

瞬Matataki最初是被当做SocialMoney（Fan票）的试验场创造出来的，以平台的身份进入内容创作这个行业算是误打误撞，因此Matataki长久以来一直对几乎所有方向 & 内容形式 的创作都抱有极高的包容度，也正是如此塑造出了 瞬Matataki 独有的气质。很多人是被基于IPFS的永久存储特性吸引过来的，阅文、马文亮、AO3 事件分别是几次重要的节点，为我们带来了很多很棒的小伙伴。我希望这样的气质可以持续保持下去，这可能就是独属于我们的内容定位。

在过去的2年中我们持续对 瞬Matataki 进行方向上的探索，我们探索留下的足迹也导致不同系统之间的耦合程度非常高。我们希望有更多的社区伙伴可以参与到Fan票和Matataki的生态建设中来，因此我们决定在足够无忧的情况下，会花费一段时间对 瞬MAtataki的整站各个模块之间完全解耦。

瞬Matataki作为内容平台功能本身还有很多的不完善，内容运营和刷存在感方面我们也没有足够的精力去顾及到。但是我们绝对不会忘记在这里还对我们保有极大期望的小伙伴们，这个产品就像是青春期的孩子，有着各种不成熟的时候，也有着各种各样的焦虑。但是我们总会长大。希望给大家带来令人满意的产品。

**小作业 ：** 在你们心目中的 瞬Matataki 是怎样的平台？欢迎在评论区将你的想法告诉我们

**附加作业：** 很多朋友反馈 瞬Matataki 这个名字不好记不好念，那么如果是你来我们取名，你会取什么名字呢？

\==所有参与小作业的伙伴们都会得到平台Fan票 META 的打赏==

***

来更新一波打赏的截图
以下的16名小伙伴都已经被打赏了 2 META 代币，当前数量非常稀少。按照稳中的方法使用[Fan票折跃门](https://matataki.io/token/in-n-out) 导出到BSC币安智能链上使用 [Unisave交易所](https://app.unisave.exchange/)交易。META代币交易 [直达链接](https://bsc-info.unisave.exchange/pair/0x3d9b56dfea016367c40e12c725a94bb09efcc3e0)

![image.png](ipfs://QmeHtR2WnQReECGTrDe6rPZJkEBieiqvEEiPzjYbQ2PT7E)

![image.png](ipfs://QmWY5safQ2X5i2Ny2VEuP24J5GgntHMGyhfSwjCwpq512U)

