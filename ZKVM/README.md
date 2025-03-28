# zkVM Course

## Background

zkVM 作为一种结合零知识证明（Zero-Knowledge Proof, ZKP）和虚拟机（Virtual Machine, VM）的新型技术，背后承载了多个领域的努力，包括密码学、区块链、分布式系统和计算理论，才走到如今，被普遍认为是突破区块链和分布式系统技术瓶颈的「潜力股」。然而，无法否认的是 zkVM 的学习较为艰难。收集了各方的需求和问题，我们发现 zkVM 的学习主要存在以下现实难题：

首先，zkVM 学习门槛相对较高。除了所用到的高级数学理论、证明系统设计以及计算的复杂性；还有为了支持通用计算，要比传统虚拟机更加复杂的设计；此外，零知识证明与虚拟机的架构要无缝结合的需求，也带来了额外的复杂性。

其次，zkVM 缺少学习材料。现在通用的 zkVM，如 Risc Zero、SP1、Miden VM、zkWASM，大部分的文档材料并不完善，并且很多关于工程类的问题难以深究，对个人来说需要耗费巨大精力，学习阻力很大。

针对上述问题，本次课程将作为学习 zkVM 系列的起步课程，后续会有更多的进阶课程。通过理论讲解和代码实践相结合的方式，从基础到进阶帮助大家全面掌握 zkVM。

## Intro

### 1. 课程时间：

2024 年 12 月 30 日 - 2015 年 1 月 27 日 （4 周）

### 2. 课程形式：

- 🧑‍🏫 线上直播授课（Zoom），每周一节课（1-1.5h/节）

- 📢 课程通知、交流讨论（微信群）

- 💬 线上答疑：https://github.com/Antalpha-Labs/zkp-academy/discussions/categories/q-a

### 3. 课程目标：

通过本期共学，参与学员将对 zkVM 形成一个高层认知，可以了解到 zkVM 的历史发展与未来的发展机会，其系统架构、虚拟机(VM) 、prover 架构设计，以及最起码会使用一个 zkVM。

## Course materials

1. [Lita - zkVM](https://www.lita.foundation/blog/zero-knowledge-paradigm-zkvm)
2. [RiscZero - zkVM](https://dev.risczero.com/api/zkvm)
3. [SP1 - zkVM](https://docs.succinct.xyz/docs/sp1/introduction)
4. [awesome-zkvm](https://github.com/rkdud007/awesome-zkvm?tab=readme-ov-file)
5. [zkMIPS](https://learnblockchain.cn/column/99)
6. [All about zkVM by Stephen Duan](https://oxidized-relation-91c.notion.site/All-about-zkVM-112f0a489b988062b4b8c51f825c2f4e)
7. [Brainfuck STARK Tutorial](https://neptune.cash/learn/brainfuck-tutorial/#wikipediaonbfdialects)

## Class schedule

【第一周课程安排】

- 第一节课：zkVM 的历史和现状
  - 讲师：wangyao，时间：12 月 31 日晚 8 点（星期二）
  - 课程回放：[Youtube 链接](https://youtu.be/xoGte-TzHHk)
  - 参考资料：
    - [A guide to Zero Knowledge Proofs](https://medium.com/@Luca_Franceschini/a-guide-to-zero-knowledge-proofs-f2ff9e5959a8) Explains basics of zkp, especially IOP and PCS.
    - [The different types of ZK-EVMs](https://vitalik.eth.limo/general/2022/08/04/zkevm.html)
    - [Jolt](https://eprint.iacr.org/2023/1217)
  - 课件：[链接](https://github.com/Antalpha-Labs/zkp-academy/blob/main/ZKVM/lesson%201/zkvm-wangyao.pdf)
- 第二节课：深入解析 Jolt
  - 讲师：Backdoor，时间：2025 年 1 月 2 日晚 8 点(星期四)
  - 课程回放：[Youtube 链接](https://youtu.be/lFUYsULyUNY)
  - 课件：[Jolt & Lasso: for Newbies](https://doutv.notion.site/Jolt-Lasso-for-Newbies-1591aee049b480b7a44ad7d00e3e9265?pvs=4)
  - 推荐阅读：[Lasso + Jolt - YouTube](https://www.youtube.com/playlist?list=PLjQ9HCQMu_8xjOEM_vh5p26ODtr-mmGxO)
    - [Binius: highly efficient proofs over binary fields](https://vitalik.eth.limo/general/2024/04/29/binius.html)
    - [Jolt - JoltBook](https://jolt.a16zcrypto.com/intro.html)
    - [Jolt R1CS - How + why we rewrote Circom in Rust 🦀](https://x.com/samrags_/status/1820429579787423759?s=46) | Sam Ragsdale
    - [A Technical Dive into Jolt: The RISC-V zkVM](https://www.zksecurity.xyz/blog/posts/how-jolt-works/)
    - [往期 jolt 学习小组视频](https://github.com/Antalpha-Labs/zkp-academy/issues/1)
- 第一周思考题（作业）：[discussion](https://github.com/Antalpha-Labs/zkp-academy/discussions/66)
- 答疑：周六晚上 8 点

【第二周课程安排】
- 第三节课：zkwasm 介绍
  - 讲师：Sinka，时间：2025年1月7日晚8点(星期二)
  - 课程回放：[Youtube 链接](https://youtu.be/ZwibS4uGEj4)
- 第四节课：zkVM 的虚拟机 (VM) 简析
  - 讲师：johnxu，时间：2025 年 1 月 9 日晚 8 点(星期四)
  - 课程回放：[Youtube 链接](https://www.youtube.com/watch?v=KxxeyKTksxs)
  - 推荐阅读:
    - [Building a RISC-V simulator in Rust](https://gregchadwick.co.uk/blog/building-rrs-pt1/)
    - [Zero Knowledge Proof — Introduction to SP1 zkVM Source Code](https://trapdoortech.medium.com/zero-knowledge-proof-introduction-to-sp1-zkvm-source-code-d26f88f90ce4)
    - [Memory management in VM](https://blog.tigris.fr/2019/07/28/writing-an-emulator-memory-management/)
    - [Writing a simple RISC-V emulator in plain C](https://fmash16.github.io/content/posts/riscv-emulator-in-c.html)
  - 课件：[链接](https://github.com/Antalpha-Labs/zkp-academy/blob/main/ZKVM/lesson%204/Introduce%20the%20zkVM.pdf)
- 第二周思考题（作业）：[discussion](https://github.com/Antalpha-Labs/zkp-academy/discussions/69)
- 答疑：周六晚上 8 点

【第三周课程安排】

- 第五节课：zkVM 电路设计与 prover 证明
  - 讲师： Dream, 时间：2025 年 1 月 14 日晚 8 点(星期二)
  - 课程回放：[Youtube](https://youtu.be/avAIjRvgwqc)
- 第六节课：zkVM 电路设计与 prover 证明
  - 讲师： Dream, 时间：2025 年 1 月 16 日晚 8 点(星期四)
  - 课程回放：[Youtube](https://youtu.be/sALgu6tHEhs)
- 答疑：周六晚上 8 点

【第四周课程安排】

- 第七节课：ZKM 的 prover 证明详解
  - 导师：Daniel，时间：2025 年 1 月 21 日晚 8 点(星期二)
  - 课程回放：[Youtube](https://youtu.be/KlhQns_8QII)
  - 课件：[链接](https://github.com/coset-io/zkp-academy/blob/main/ZKVM/lesson%207/ZKM%20Prover%E5%9F%BA%E6%9C%AC%E6%9E%84%E9%80%A0%E8%AF%BE%E7%A8%8B.pptx)
- 第八节课：zkVM 实操讲解
  - 导师：johnxu，时间：2025 年 1 月 23 日晚 8 点(星期四)
  - 课程回放：[Youtube](https://youtu.be/rSNyOY1U7x0)
- 答疑：周六晚上 8 点

【课后作业】
@所有人 本期课程全部结束🎉，目前有四个作业给到大家，其实也是思考题，大家可以挑选任意一个（里面的任何一个问题）解答，这些问题也是帮助大家更了解zkVM，提前祝大家过节好呀🧧！
[第一周作业](https://github.com/coset-io/zkp-academy/discussions/66)

[第二周作业](https://github.com/coset-io/zkp-academy/discussions/69)

[zkVM课程作业(三)Add instruction in SP1](https://github.com/coset-io/zkp-academy/discussions/70)

[zkVM系列课程作业(四) 性能分析](https://github.com/coset-io/zkp-academy/discussions/71)


## Mentors & Assistants

- **Dream:** 前 Scroll Core Engineer, Blocksight 作者。数学&密码学持续学习者，前爱立信，微软高级工程师，区块链与隐私计算一线工程研发。
- **wangyao:** fluent zk 工程师。数学博士（未完成）研究 ZK，学习 FHE，探索代数学和密码学的相交地带。
- **郭宇:** SECBIT Labs （安比实验室）创始人，曾经高校教育从业者，关注领域为零知识证明，智能合约安全，程序语言理论。
- **backdoor:** OKX ZK Dev，代码和理论两手抓，希望跟大家多交流学习～
- **johnxu:** zk 和 rust 爱好者， 密码学工程师
- **Daniel:** 浙江大学博士后研究员，密码学博士，曾在 NDSS，TIFS 等旗舰会议和期刊发表多篇论文，主要研究方向为安全多方计算和零知识证明。
- **Harold:** 研究 zk 协议 todolist 望不到头的人，偶尔会做一些技术分享，欢迎大家来一起讨论～
- **Kyrin:** 区块链方向博士，zkp 技术爱好者，与大佬们学习最新技术。

## Co-learning bounty

- 为鼓励学员学习与分享，本课程继续 Co-learn notes bounty 活动，学员可以将学习中的内容整理成个人笔记提交到 [co-learn notes](https://github.com/Antalpha-Labs/zkp-academy/tree/main/ZKVM/co-learn-notes) 目录下，收录后每篇笔记给出 200 CNY 的 bounty，并发布在 Coset 公众号上。

- 报名助教，积极回答技术问题，推动学员一起学习，不止退回押金，还可以收获 200 CNY 的 bounty。

\*笔记主题围绕 ZKP 相关技术，不局限于 zkVM。

**联系方式**：添加小助手微信 Coset2025

## Sponsor

<img src="assets/ZKM Logo Horizontal Black-1.png" width="75%;"/>
