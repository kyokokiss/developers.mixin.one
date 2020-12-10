# EOS

EOS（Enterprise Operation System）是一个高性能的商用区块链操作系统。

### 基本信息

- 主网上线：2018/06/15
- 共识机制：DPoS + BFT
- 主网代币：EOS（EOS）
- 最大发行：无上限，通胀模型，年增发 1%
- 出块时间：0.5 秒
- 区块大小：1M
- 不可逆块：[约为 335 区块](https://eosflare.io/)
- 交易数据：38 亿（截止到 2020/11/26）
- 发币功能：有
- 核心人物：Dan Larimer（BM）

### 主网特点

- 高性能

  基于有限的节点数量、石墨烯技术和并行链可实现毫秒级确认和百万 TPS，满足大型商业级需求。

- 转账免费

  转账免费，代币不会在转账时消耗，用抵押替代消耗。
  
- 更友好的账户

  相比比特币和以太坊一长串字符串 EOS 的账户用户名大大提升了可读性，使用更便利。

### 核心概念

EOS 模拟了真实计算机的大多数属性，包括 CPU﹑内存﹑硬盘存储等，计算机资源将平均分配给 EOS 代币的持有人。

- DPoS

  EOS 采用去中心化共识算法委托权益证明 Delegated Proof of Stake (DPOS)，持有 EOS 的人通过投票系统选出区块生产者，任何人都可以选择参加区块生产，只要能够说服通证持有人为其投票，就会有机会参与区块生产。

- 账户

  所有的账户都由一个唯一名称来标识，用户名的最大长度为 12 个字符，包括 `a-z` 以及 `1-5`，不含 `0`，新用户注册时需要支付账号创建费用，低于 12 个字符的用户名需要通过竞拍获得。

  所有账户默认指定两个权限组：一个是 `owner` 权限组，可以执行任何操作；另一个 `active` 权限组，除了更改 `owner` 权限组之外，可以执行所有操作。所有其他权限组均由 `active` 组派生。
  
  可通过指定帐户恢复合作伙伴，在账号被盗之后重置账号的 owner 密钥。

  所有超级节点有权冻结冻结账号和交易，例如某个应用程序或账户的某个行为会导致其过度消耗资源，且问题不可避免地发生时，区块生产者有权去纠正这些问题，需要 21 个活跃生产者中的 15 个投票达成一致。

- CPU

  计算资源负责处理事务，通过抵押 EOS、第三方代付或 REX（EOS 系统级资源租赁系统） 租赁获得。

- 带宽（NET）

  带宽资源用于传输数据，通过抵押 EOS 获得，所有交易会根据执行的 WASM 指令数来计算带宽成本。

- 内存（RAM）

  RAM 用于存储区块链中的数据，必须通过 EOS 购买获得，创建账号、转账、购买资源、抵押、赎回、投票等操作都可能要消耗 RAM，RAM 的价格是基于 Bancor 算法由市场决定。

- 智能合约

  开发者可以很方便用 C、C++、Rust 编写合约代码，然后编译成 WebAssembly（WASM）格式的字节码在 EOS 平台上的 WASM 虚拟机上运行。

  合约可升级，方便开发者及时修复错误，但同时也带来了可随时升级合约卷跑跑路的风险，可通过多签来改善这个问题。

- 石墨烯技术（Graphene Blockchain Technology）

  用 C++ 语言编写，具有转账速度快、吞吐量高、稳定性强、功能完备、易操作等特性，曾应用于 BitShares、Steem 和 GXChain 等。

### 常用网址

- https://eosflare.io/

  EOS 区块链浏览器

### 小知识

- Block.one、EOS.IO 和 EOS 什么关系？

  Block.one 是一家软件公司，主导开发了免费、开源的 EOS.IO 软件平台，社区用 EOS.IO 启动了 EOS 主网。