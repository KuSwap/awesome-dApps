# awesome-dApps

English | [简体中文](README_CN.md)


## How to add a dApp

The source data is in the _data/dapps. Each dApp has its own file, the file name is composed of PR number, project name and .json, such as: 1_uniswap_v2.json

1. Fork this project to your own GitHub repository (so you have a copy on your own GitHub account).
2. Create a branch in your own repository (this time the origin will be your own fork, not the public one).
3. Modify the site code locally and complete the tests.
4. Commit the changes to your branch.
5. Push the changes to your main branch.
6. Create a Pull Request (PR) on GitHub (awesome-dApps ← your own GitHub).

When the PR is submitted, it will be reviewed and, if accepted, merged into the main branch. If you have any questions, you can send an e-mail to [kcc-tech@kcc.network](mailto:kcc-tech@kcc.network).


## dApp Requests

- You need to add crucial dApp information, including but not limited to **name**, **logo**, **description**, **category**, **website**, **audit reports**, **smart contracts**, **social links**. No GitHub link, no audit pass.
- The added dApp must be published on **mainnet** or **testnet**.
- The logo image needs to be uploaded to **IPFS**, which can be **png**, **jpg**, **svg**, and the image size is uniformly 256*256
- The newly added item should be added to the end of the dApps list, otherwise the audit will not pass.


## dApp Example

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