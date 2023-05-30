# OK链（OKC okchain） 币安链(BSC) 抢跑机器人
## 监控内存池, 发现套利机会，用更高的gas fee抢跑, 然后套取利润 (2023年5月最新版)
## 支持FTM POLYGON 以太坊 Arbiscan Snowtrace MoonRiver Cronos
## okc bnb由于竞争激烈，每日获利已低于5 USDT 我已经有了更好的商业模式，不再需要进行简单的套利了，发布出来主要是为了打脸一下那些质疑我的人。

## 原理
机器人发送Transaction 去监控 Uniswap 内存池，发现有大单交易，会导致滑点产生，就有了套利机会

然后，机器人抢在他之前购买链上的代币，随后卖出，获得滑点利润

最后从合约中提取利润.

比市面上99%的机器人还要快.

https://www.zvstus.com/article/news/1/75d87ffffe86e2af46b35601f0180000.html

## 别人已经开源过了
是的，别人有开源的，但我的更快。我读过所有的关于套利的资料，不断的代码改进使我的bot更快 <3

## 如何领先其他人 ?
我在这个项目上花了一年时间， 我知道别的BOT的IP地址，所以可以ddos他们，使得他们比我慢一点.
体会
## 我学到了什么?
MEV套利知识, Frontrunning抢跑, EIP-1559, “黑暗森林”，各种利用更多 web3 的技巧. 以及关于 Uniswap 或 Pancakeswap 的各种细节.
为什么我不继续了?
我从中获得了一些利润，但现在使用其他一些更好的商业方法，这些微薄的利润我不再需要，分享我学到的东西，这样其他人就不需要经历同样的痛苦。

其他链上的成果:

https://etherscan.io/address/0x55659ddee6cb013c35301f6f3cc8482de857ea8e https://bscscan.com/address/0x55659ddee6cb013c35301f6f3cc8482de857ea8e

## 注意：

bsc gas fee最好不要低于0.1 套利amount 0.2

测试网测试需要填写正确的测试网usdt等地址

套利需要等一段时间才能获得收益，因为不是时时刻刻都存在套利机会

## 如何部署
打开合约部署地址: https://remix.ethereum.org/

单击“contracts”文件夹，然后创建“New File”。 根据需要重命名，比如：“bot.sol”

将名称为 bot.sol 中的代码粘贴到 remix 中

在“Solidity Compiler”选项卡，选择“0.6.6”或“0.6.12”版本，然后“编译”它。

移至“部署”选项卡，选择“Injected Web 3”环境。 将你的 Metamask 与 Remix 连接，然后“部署合约。 交易确认后，你就拥有你自己的BOT了。

将初始套利资金(原生代币)存入您的合约地址（给合约存入okt、bnb等用于套利资金和gas fee）,gas fee不能太少，容易耗尽导致交易失败或者达不到套利条件

存入资金后, 点击 “start” 按钮. 如果想提取资金，点击“withdrawal” 按钮取回

代码仅供参考，在运行代码套利的过程中，发生资金风险，自行承担