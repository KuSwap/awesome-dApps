# awesome-dApps

[English](README.md) | 简体中文


## dApp 添加

源码在_data/dapps目录。每个dApp有自己的文件，文件名由PR编号、项目名称和.json组成，如：1_uniswap_v2.json

1. Fork 这个项目到自己的 GitHub 仓库，相当于拷贝一份到自己的 GitHub 账户下
2. 将自己的库 Pull 下来（这时候 Origin 是自己的地址，不是公共地址）
3. 创建子分支，在_data/dapps目录下增加文件，并完成测试
4. 提交修改（Commit）
5. Push 到自己的 GitHub，也就是当前的 Origin 地址
6. 在 GitHub 上提交 Pull request（awesome-dApps ← Your GitHub）

提交 Pull request 后，管理员审核通过后，就会合并到主分支中。若有疑问，可以发邮件到 [kcc-tech@kcc.network](mailto:kcc-tech@kcc.network)


## dApp 要求

- 需要添加完善的 dApp 信息，包括但不限于 **名称**、**logo**、**描述**、**类别**、**官网**、**审计报告**、**智能合约**、**社交网络**，没有 GitHub 的项目将不被审核通过
- 所添加的 dApp 必需已在 **mainnet** 或 **testnet** 上发布
- logo图片需上传至 **IPFS**，可以是**png**、**jpg**、**svg**，图片尺寸统一使用256*256
- 新添加的项目应该添加到项目列表的最后，否则审核不会通过


## dApp 示例

```json
{
    "name": "Uniswap V2", 
    "logo": "https://ipfs.io/ipfs/QmWoRyyU7N16irq9xL6x9kwj6kMmWZgVE12kcCJZZH6y9e", 
    "description": "A protocol for trading and automated liquidity provision on Ethereum.", 
    "category": "exchange", 
    "website": "https://app.uniswap.org/#/swap", 
    "audit": "https://uniswap.org/audit.html", 
    "contracts": [
        {
            "remark": "UniswapV2Router02", 
            "address": "0x7a250d5630B4cF539739dF2C5dAcb4c659F2488D"
        }
    ], 
    "links": [
        {
            "type": "twitter", 
            "url": "https://twitter.com/Uniswap"
        }, 
        {
            "type": "reddit", 
            "url": "https://www.reddit.com/r/UniSwap"
        }, 
        {
            "type": "github", 
            "url": "https://github.com/Uniswap"
        }, 
        {
            "type": "blog", 
            "url": "https://uniswap.org/blog/"
        }
    ]
}
```