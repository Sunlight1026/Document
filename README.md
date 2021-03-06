# Document (DQMT)

Document ideas and items on the ethereum classic blockchain using an NFT smart contract.  This smart contract is
an easy way for users to interact with the ETC blockchain.  Web interface is still under construction but the contract
is fully functional and accessible via the instructions below. We've written an article at Medium.com explaining how to 
deploy your own erc721 token using this smart contract as an example.  [View it on Medium](https://medium.com/@danpittman_41978/building-an-erc721-non-fungible-token-smart-contract-and-using-metamask-to-interact-with-it-via-a-59583f0dd6c1) 
or [View it on Steemit](https://steemit.com/erc721/@Sunlight1026/building-an-erc721-non-fungible-token-smart-contract-and-using-metamask-to-interact-with-it-via-a-web-interface-part-i)

## Getting Started

The easiest way of accessing the buyToken function which allows you to create a post on the ethereum blockchain is to visit
[Sunlight1026](https://Sunlight1026.io/document).  We are currently using the Ropsten testnet so please make sure metamask is connected to
Ropsten instead of the main network.  To use the full functionality of the contract on the ETC blockchain please use the instructions
below:


Access DQMT at [Ethereum Classic Wallet](https://ethereumproject.github.io/etherwallet/) or Parity
using the parameters below.

```
#Contract address on the ETC Blockchain
0xB12Bbc6D3E451fBC56f813297E314A5F8E118028
```

```
ABI/JSON Interface:
```
```
[{"constant":true,"inputs":[{"name":"_interfaceId","type":"bytes4"}],"name":"supportsInterface","outputs":
[{"name":"","type":"bool"}],"payable":false,"stateMutability":"view","type":"function"},{"constant":true,
"inputs":[],"name":"name","outputs":[{"name":"","type":"string"}],"payable":false,"stateMutability":"view",
"type":"function"},{"constant":true,"inputs":[{"name":"_tokenId","type":"uint256"}],"name":"getApproved",
"outputs":[{"name":"","type":"address"}],"payable":false,"stateMutability":"view","type":"function"},
{"constant":false,"inputs":[{"name":"_to","type":"address"},{"name":"_tokenId","type":"uint256"}],"name":"approve",
"outputs":[],"payable":false,"stateMutability":"nonpayable","type":"function"},{"constant":true,"inputs":[],
"name":"totalSupply","outputs":[{"name":"","type":"uint256"}],"payable":false,"stateMutability":"view","type":"function"},
{"constant":false,"inputs":[{"name":"newPrice","type":"uint256"}],"name":"setCurrentPrice","outputs":[],
"payable":false,"stateMutability":"nonpayable","type":"function"},{"constant":true,"inputs":[],"name":"InterfaceId_ERC165",
"outputs":[{"name":"","type":"bytes4"}],"payable":false,"stateMutability":"view","type":"function"},
{"constant":false,"inputs":[{"name":"_from","type":"address"},{"name":"_to","type":"address"},{"name":"_tokenId","type":"uint256"}],
"name":"transferFrom","outputs":[],"payable":false,"stateMutability":"nonpayable","type":"function"},
{"constant":true,"inputs":[{"name":"_owner","type":"address"},{"name":"_index","type":"uint256"}],
"name":"tokenOfOwnerByIndex","outputs":[{"name":"","type":"uint256"}],"payable":false,"stateMutability":"view","type":"function"},
{"constant":false,"inputs":[{"name":"_from","type":"address"},{"name":"_to","type":"address"},{"name":"_tokenId","type":"uint256"}],
"name":"safeTransferFrom","outputs":[],"payable":false,"stateMutability":"nonpayable","type":"function"},{"constant":true,"inputs":
[{"name":"_tokenId","type":"uint256"}],"name":"exists","outputs":[{"name":"","type":"bool"}],"payable":false,"stateMutability":
"view","type":"function"},{"constant":true,"inputs":[{"name":"_index","type":"uint256"}],"name":"tokenByIndex","outputs":
[{"name":"","type":"uint256"}],"payable":false,"stateMutability":"view","type":"function"},{"constant":false,"inputs":[{"name":
"_type","type":"uint256"},{"name":"_title","type":"string"},{"name":"_description","type":"string"}],"name":"buyToken","outputs":[],
"payable":true,"stateMutability":"payable","type":"function"},{"constant":true,"inputs":[{"name":"_tokenId","type":"uint256"}],
"name":"ownerOf","outputs":[{"name":"","type":"address"}],"payable":false,"stateMutability":"view","type":"function"},{"constant":true,
"inputs":[{"name":"_owner","type":"address"}],"name":"balanceOf","outputs":[{"name":"","type":"uint256"}],"payable":false,"stateMutability":
"view","type":"function"},{"constant":false,"inputs":[],"name":"renounceOwnership","outputs":[],"payable":false,"stateMutability":
"nonpayable","type":"function"},{"constant":true,"inputs":[],"name":"owner","outputs":[{"name":"","type":"address"}],"payable":false,
"stateMutability":"view","type":"function"},{"constant":true,"inputs":[],"name":"myTokens","outputs":[{"name":"","type":"uint256[]"}],
"payable":false,"stateMutability":"view","type":"function"},{"constant":true,"inputs":[],"name":"symbol","outputs":[{"name":"",
"type":"string"}],"payable":false,"stateMutability":"view","type":"function"},{"constant":false,"inputs":[{"name":"_to","type":"address"},
{"name":"_approved","type":"bool"}],"name":"setApprovalForAll","outputs":[],"payable":false,"stateMutability":"nonpayable","type":"function"},
{"constant":false,"inputs":[{"name":"_from","type":"address"},{"name":"_to","type":"address"},{"name":"_tokenId","type":"uint256"},
{"name":"_data","type":"bytes"}],"name":"safeTransferFrom","outputs":[],"payable":false,"stateMutability":"nonpayable","type":"function"},
{"constant":true,"inputs":[{"name":"_tokenId","type":"uint256"}],"name":"tokenURI","outputs":[{"name":"","type":"string"}],
"payable":false,"stateMutability":"view","type":"function"},{"constant":true,"inputs":[{"name":"_tokenId","type":"uint256"}],
"name":"getToken","outputs":[{"name":"tokenType_","type":"uint256"},{"name":"tokenTitle_","type":"string"},{"name":"tokenDescription_",
"type":"string"}],"payable":false,"stateMutability":"view","type":"function"},{"constant":true,"inputs":[{"name":"_owner","type":"address"},
{"name":"_operator","type":"address"}],"name":"isApprovedForAll","outputs":[{"name":"","type":"bool"}],"payable":false,"stateMutability":
"view","type":"function"},{"constant":true,"inputs":[],"name":"getCurrentPrice","outputs":[{"name":"price","type":"uint256"}],
"payable":false,"stateMutability":"view","type":"function"},{"constant":false,"inputs":[{"name":"_newOwner","type":"address"}],
"name":"transferOwnership","outputs":[],"payable":false,"stateMutability":"nonpayable","type":"function"},{"inputs":[],
"payable":false,"stateMutability":"nonpayable","type":"constructor"},{"anonymous":false,"inputs":[{"indexed":true,"name":"buyer","type":
"address"},{"indexed":false,"name":"tokenId","type":"uint256"}],"name":"BoughtToken","type":"event"},{"anonymous":false,"inputs":
[{"indexed":true,"name":"previousOwner","type":"address"}],"name":"OwnershipRenounced","type":"event"},{"anonymous":false,"inputs":[{
"indexed":true,"name":"previousOwner","type":"address"},{"indexed":true,"name":"newOwner","type":"address"}],"name":"OwnershipTransferred",
"type":"event"},{"anonymous":false,"inputs":[{"indexed":true,"name":"_from","type":"address"},{"indexed":true,"name":"_to",
"type":"address"},{"indexed":true,"name":"_tokenId","type":"uint256"}],"name":"Transfer","type":"event"},{"anonymous":false,
"inputs":[{"indexed":true,"name":"_owner","type":"address"},{"indexed":true,"name":"_approved","type":"address"},{"indexed":true,
"name":"_tokenId","type":"uint256"}],"name":"Approval","type":"event"},{"anonymous":false,"inputs":[{"indexed":true,"name":
"_owner","type":"address"},{"indexed":true,"name":"_operator","type":"address"},{"indexed":false,"name":"_approved","type":"bool"}],
"name":"ApprovalForAll","type":"event"}]
```
There are many functions available but the one that may interest you the most will be the```buyToken```function.  The tokens are free 
but you will need to send some gas when executing the contract.  We built this dApp on the ETC blockchain so the gas price would stay low.

```

List of available functions
#Purchase a token -  this command will cost you gas
#You will be required to name the tokenId when creating a token.  
#Please type 1 for Ideas or 2 for Items.
#Give your idea/item a title
#Give your idea/item a description
buyToken


#View ideas or items
getToken

```

## Contributing

Please read [CONTRIBUTING.md](https://github.com/Sunlight1026/Document/contributing.md) for details on our code of conduct, and the process for submitting pull requests to us.

## Authors

* **Daniel Pittman**             - [Sunlight1026](https://www.Sunlight1026.io) - [LinkedIn](https://www.linkedin.com/in/mrpittman1/) - [Twitter](https://www.twitter.com/Sunlight1026)
* **Bill Morris**   

See also the list of [contributors](https://github.com/Sunlight1026/Document/contributors) who participated in this project.

## License

This project is licensed under the Apache 2.0 - see the [LICENSE.md](LICENSE.md) file for details

## Acknowledgments

  Big Thanks to 
* chuckbergeron
* ethereum core

### Donate

If you like our project please contribute by donating 

ETC: 0x007e60C669cf96dC32655d1Eb1c1eBcf96459975

BTC: 15X8rjV7EaTtsC6BhrffuqH28LZpqZ9Tdi

BCC: 1KrwR96hbCrLavAaWkXz2oy2F51ryohme1

ETH: 0x00c24b3346AFc5c3710AFb27C86431ebB5ce8163