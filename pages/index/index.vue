<template>
	<view class="content">
		<view class="bg" >
			<view class="uni-flex uni-row" style="margin: 1.625rem; height: 89.44rpx;">
			<img class="flex-item" src="../../static/heard.png" style="width:3.125rem;" />
			<img class="currentImg" src="../../static/Ellipse38.png" />
			<view class="currentbs"  >在线3000步</view>
			<img class="userName" src="../../static/Group3.png" />
			</view>
			
			<view class="person">
				<img class="gp11 gp12" src="../../static/Group11.png" />
				<img class="gp12" src="../../static/Group12070.png" />
				<img class="gp12" src="../../static/Group12071.png" />
			</view>
			
			<img class="gp5" src="../../static/Group5-1.png" />
			
						<uni-card title="" extra="" style="width: 70%; margin: 0.625rem auto;">
							<view class="uni-flex uni-row">
								<img class="currentImg2" src="../../static/Vector14.png" />
								
								<view class="uni-flex uni-column">
								
								<view class="curId uni-flex uni-row" > 
									<view class="flex-item " >ID</view>
									<view class="flex-item idvalue" >10320</view>
								</view>
								
								<view class="curId uni-flex uni-row" >
									<view class="flex-item " >Name</view>
									<view class="flex-item idvalue" >xx</view>
								</view>
								<view class="curId uni-flex uni-row" >
									<view class="flex-item " >Level</view>
									<view class="idvalue" >1</view>
								</view>
								</view>
								
							</view>
							
						</uni-card>
					
								<uni-card title="" extra="" style="width: 70%; margin: 0.225rem auto;">
									<view class="uni-flex uni-row">
										<img class="currentImg2" src="../../static/Vector14.png" />
										
										<view class="uni-flex uni-column">
										
										<view class="curId uni-flex uni-row" >
											<view class="flex-item " >预计收益</view>
											<view class="flex-item idvalue2" >10000</view>
										</view>
										
										</view>
										
									</view>
									
								</uni-card>
							
							<img class="gp4" src="../../static/Group4.png" />
							
							<view class="bs">已同步1000步</view>
			
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				value:"",
				title: 'Hello',
				 layerAbi: [{
					"inputs": [{
						"internalType": "address",
						"name": "_token",
						"type": "address"
					}, {
						"internalType": "address",
						"name": "_recipient",
						"type": "address"
					}, {
						"internalType": "address",
						"name": "_NFTAddress",
						"type": "address"
					}],
					"stateMutability": "nonpayable",
					"type": "constructor"
				}, {
					"anonymous": false,
					"inputs": [{
						"indexed": true,
						"internalType": "address",
						"name": "from",
						"type": "address"
					}, {
						"indexed": true,
						"internalType": "uint256",
						"name": "amount",
						"type": "uint256"
					}],
					"name": "BuyRB",
					"type": "event"
				}, {
					"anonymous": false,
					"inputs": [{
						"indexed": true,
						"internalType": "address",
						"name": "from",
						"type": "address"
					}, {
						"indexed": false,
						"internalType": "address",
						"name": "to",
						"type": "address"
					}, {
						"indexed": true,
						"internalType": "uint256",
						"name": "amount",
						"type": "uint256"
					}],
					"name": "Devidend",
					"type": "event"
				}, {
					"anonymous": false,
					"inputs": [{
						"indexed": true,
						"internalType": "address",
						"name": "to",
						"type": "address"
					}, {
						"indexed": false,
						"internalType": "string",
						"name": "date",
						"type": "string"
					}, {
						"indexed": false,
						"internalType": "uint256",
						"name": "amount",
						"type": "uint256"
					}],
					"name": "InCome",
					"type": "event"
				}, {
					"anonymous": false,
					"inputs": [{
						"indexed": true,
						"internalType": "address",
						"name": "from",
						"type": "address"
					}, {
						"indexed": false,
						"internalType": "address",
						"name": "to",
						"type": "address"
					}, {
						"indexed": true,
						"internalType": "uint256",
						"name": "amount",
						"type": "uint256"
					}],
					"name": "PromotionAward",
					"type": "event"
				}, {
					"anonymous": false,
					"inputs": [{
						"indexed": true,
						"internalType": "address",
						"name": "to",
						"type": "address"
					}, {
						"indexed": false,
						"internalType": "address",
						"name": "from",
						"type": "address"
					}],
					"name": "ReferrerAdded",
					"type": "event"
				}, {
					"anonymous": false,
					"inputs": [{
						"indexed": true,
						"internalType": "bytes32",
						"name": "role",
						"type": "bytes32"
					}, {
						"indexed": true,
						"internalType": "bytes32",
						"name": "previousAdminRole",
						"type": "bytes32"
					}, {
						"indexed": true,
						"internalType": "bytes32",
						"name": "newAdminRole",
						"type": "bytes32"
					}],
					"name": "RoleAdminChanged",
					"type": "event"
				}, {
					"anonymous": false,
					"inputs": [{
						"indexed": true,
						"internalType": "bytes32",
						"name": "role",
						"type": "bytes32"
					}, {
						"indexed": true,
						"internalType": "address",
						"name": "account",
						"type": "address"
					}, {
						"indexed": true,
						"internalType": "address",
						"name": "sender",
						"type": "address"
					}],
					"name": "RoleGranted",
					"type": "event"
				}, {
					"anonymous": false,
					"inputs": [{
						"indexed": true,
						"internalType": "bytes32",
						"name": "role",
						"type": "bytes32"
					}, {
						"indexed": true,
						"internalType": "address",
						"name": "account",
						"type": "address"
					}, {
						"indexed": true,
						"internalType": "address",
						"name": "sender",
						"type": "address"
					}],
					"name": "RoleRevoked",
					"type": "event"
				}, {
					"anonymous": false,
					"inputs": [{
						"indexed": true,
						"internalType": "address",
						"name": "from",
						"type": "address"
					}, {
						"indexed": true,
						"internalType": "address",
						"name": "to",
						"type": "address"
					}, {
						"indexed": false,
						"internalType": "uint256",
						"name": "amount",
						"type": "uint256"
					}],
					"name": "TransferToken",
					"type": "event"
				}, {
					"inputs": [],
					"name": "DEFAULT_ADMIN_ROLE",
					"outputs": [{
						"internalType": "bytes32",
						"name": "",
						"type": "bytes32"
					}],
					"stateMutability": "view",
					"type": "function"
				}, {
					"inputs": [{
						"internalType": "address",
						"name": "",
						"type": "address"
					}],
					"name": "Details",
					"outputs": [{
						"internalType": "uint256",
						"name": "numTimes",
						"type": "uint256"
					}, {
						"internalType": "uint256",
						"name": "amount",
						"type": "uint256"
					}, {
						"internalType": "bool",
						"name": "isUsed",
						"type": "bool"
					}],
					"stateMutability": "view",
					"type": "function"
				}, {
					"inputs": [{
						"internalType": "string",
						"name": "",
						"type": "string"
					}],
					"name": "Incomes",
					"outputs": [{
						"internalType": "uint256",
						"name": "numTimes",
						"type": "uint256"
					}, {
						"internalType": "uint256",
						"name": "amount",
						"type": "uint256"
					}, {
						"internalType": "bool",
						"name": "isUsed",
						"type": "bool"
					}, {
						"internalType": "bool",
						"name": "isDealed",
						"type": "bool"
					}],
					"stateMutability": "view",
					"type": "function"
				}, {
					"inputs": [],
					"name": "NFTAddress",
					"outputs": [{
						"internalType": "address",
						"name": "",
						"type": "address"
					}],
					"stateMutability": "view",
					"type": "function"
				}, {
					"inputs": [{
						"internalType": "address",
						"name": "",
						"type": "address"
					}],
					"name": "UserRBTotal",
					"outputs": [{
						"internalType": "uint256",
						"name": "",
						"type": "uint256"
					}],
					"stateMutability": "view",
					"type": "function"
				}, {
					"inputs": [{
						"internalType": "address",
						"name": "from",
						"type": "address"
					}, {
						"internalType": "address",
						"name": "to",
						"type": "address"
					}],
					"name": "addReferrer",
					"outputs": [],
					"stateMutability": "nonpayable",
					"type": "function"
				}, {
					"inputs": [{
						"internalType": "address",
						"name": "",
						"type": "address"
					}, {
						"internalType": "uint256",
						"name": "",
						"type": "uint256"
					}],
					"name": "bonusDetail",
					"outputs": [{
						"internalType": "uint256",
						"name": "time",
						"type": "uint256"
					}, {
						"internalType": "uint256",
						"name": "amount",
						"type": "uint256"
					}],
					"stateMutability": "view",
					"type": "function"
				}, {
					"inputs": [{
						"internalType": "uint256",
						"name": "Rbnum",
						"type": "uint256"
					}],
					"name": "buyRB",
					"outputs": [],
					"stateMutability": "nonpayable",
					"type": "function"
				}, {
					"inputs": [{
						"internalType": "address",
						"name": "",
						"type": "address"
					}, {
						"internalType": "uint256",
						"name": "",
						"type": "uint256"
					}],
					"name": "buyRBStatus",
					"outputs": [{
						"internalType": "bool",
						"name": "",
						"type": "bool"
					}],
					"stateMutability": "view",
					"type": "function"
				}, {
					"inputs": [{
						"internalType": "uint256",
						"name": "",
						"type": "uint256"
					}],
					"name": "cards",
					"outputs": [{
						"internalType": "uint256",
						"name": "index",
						"type": "uint256"
					}, {
						"internalType": "string",
						"name": "uri",
						"type": "string"
					}],
					"stateMutability": "view",
					"type": "function"
				}, {
					"inputs": [{
						"internalType": "string",
						"name": "",
						"type": "string"
					}, {
						"internalType": "uint256",
						"name": "",
						"type": "uint256"
					}],
					"name": "class1",
					"outputs": [{
						"internalType": "address",
						"name": "",
						"type": "address"
					}],
					"stateMutability": "view",
					"type": "function"
				}, {
					"inputs": [{
						"internalType": "string",
						"name": "date",
						"type": "string"
					}],
					"name": "class1Length",
					"outputs": [{
						"internalType": "uint256",
						"name": "",
						"type": "uint256"
					}],
					"stateMutability": "view",
					"type": "function"
				}, {
					"inputs": [{
						"internalType": "string",
						"name": "",
						"type": "string"
					}, {
						"internalType": "uint256",
						"name": "",
						"type": "uint256"
					}],
					"name": "class2",
					"outputs": [{
						"internalType": "address",
						"name": "",
						"type": "address"
					}],
					"stateMutability": "view",
					"type": "function"
				}, {
					"inputs": [{
						"internalType": "string",
						"name": "date",
						"type": "string"
					}],
					"name": "class2Length",
					"outputs": [{
						"internalType": "uint256",
						"name": "",
						"type": "uint256"
					}],
					"stateMutability": "view",
					"type": "function"
				}, {
					"inputs": [{
						"internalType": "string",
						"name": "",
						"type": "string"
					}, {
						"internalType": "uint256",
						"name": "",
						"type": "uint256"
					}],
					"name": "class3",
					"outputs": [{
						"internalType": "address",
						"name": "",
						"type": "address"
					}],
					"stateMutability": "view",
					"type": "function"
				}, {
					"inputs": [{
						"internalType": "string",
						"name": "date",
						"type": "string"
					}],
					"name": "class3Length",
					"outputs": [{
						"internalType": "uint256",
						"name": "",
						"type": "uint256"
					}],
					"stateMutability": "view",
					"type": "function"
				}, {
					"inputs": [{
						"internalType": "string",
						"name": "",
						"type": "string"
					}, {
						"internalType": "address",
						"name": "",
						"type": "address"
					}],
					"name": "classList",
					"outputs": [{
						"internalType": "uint256",
						"name": "",
						"type": "uint256"
					}],
					"stateMutability": "view",
					"type": "function"
				}, {
					"inputs": [],
					"name": "clearClass",
					"outputs": [],
					"stateMutability": "nonpayable",
					"type": "function"
				}, {
					"inputs": [{
						"internalType": "string",
						"name": "",
						"type": "string"
					}],
					"name": "dayLimit",
					"outputs": [{
						"internalType": "uint256",
						"name": "",
						"type": "uint256"
					}],
					"stateMutability": "view",
					"type": "function"
				}, {
					"inputs": [{
						"internalType": "int256",
						"name": "timestamp",
						"type": "int256"
					}, {
						"internalType": "int8",
						"name": "timezone",
						"type": "int8"
					}],
					"name": "daysToDate",
					"outputs": [{
						"internalType": "uint256",
						"name": "year",
						"type": "uint256"
					}, {
						"internalType": "uint256",
						"name": "month",
						"type": "uint256"
					}, {
						"internalType": "uint256",
						"name": "day",
						"type": "uint256"
					}],
					"stateMutability": "pure",
					"type": "function"
				}, {
					"inputs": [{
						"internalType": "int256",
						"name": "timestamp",
						"type": "int256"
					}, {
						"internalType": "int8",
						"name": "timezone",
						"type": "int8"
					}],
					"name": "daysToDateString",
					"outputs": [{
						"internalType": "string",
						"name": "dateTime",
						"type": "string"
					}],
					"stateMutability": "pure",
					"type": "function"
				}, {
					"inputs": [{
						"internalType": "string",
						"name": "",
						"type": "string"
					}],
					"name": "dealStatus",
					"outputs": [{
						"internalType": "bool",
						"name": "",
						"type": "bool"
					}],
					"stateMutability": "view",
					"type": "function"
				}, {
					"inputs": [{
						"internalType": "address",
						"name": "",
						"type": "address"
					}],
					"name": "dealTimeList",
					"outputs": [{
						"internalType": "uint256",
						"name": "",
						"type": "uint256"
					}],
					"stateMutability": "view",
					"type": "function"
				}, {
					"inputs": [],
					"name": "dividend",
					"outputs": [],
					"stateMutability": "nonpayable",
					"type": "function"
				}, {
					"inputs": [{
						"internalType": "string",
						"name": "",
						"type": "string"
					}],
					"name": "dividendByDayList",
					"outputs": [{
						"internalType": "uint256",
						"name": "class1",
						"type": "uint256"
					}, {
						"internalType": "uint256",
						"name": "class2",
						"type": "uint256"
					}, {
						"internalType": "uint256",
						"name": "class3",
						"type": "uint256"
					}],
					"stateMutability": "view",
					"type": "function"
				}, {
					"inputs": [{
						"internalType": "address",
						"name": "userAddress",
						"type": "address"
					}],
					"name": "dividendOf",
					"outputs": [{
						"internalType": "uint256",
						"name": "",
						"type": "uint256"
					}],
					"stateMutability": "view",
					"type": "function"
				}, {
					"inputs": [],
					"name": "getBonus",
					"outputs": [],
					"stateMutability": "nonpayable",
					"type": "function"
				}, {
					"inputs": [{
						"internalType": "address",
						"name": "_addr",
						"type": "address"
					}],
					"name": "getBonusDetailList",
					"outputs": [{
						"components": [{
							"internalType": "uint256",
							"name": "time",
							"type": "uint256"
						}, {
							"internalType": "uint256",
							"name": "amount",
							"type": "uint256"
						}],
						"internalType": "struct Layer.Bonus[]",
						"name": "",
						"type": "tuple[]"
					}],
					"stateMutability": "view",
					"type": "function"
				}, {
					"inputs": [{
						"internalType": "string",
						"name": "date",
						"type": "string"
					}],
					"name": "getClass1List",
					"outputs": [{
						"internalType": "address[]",
						"name": "",
						"type": "address[]"
					}],
					"stateMutability": "view",
					"type": "function"
				}, {
					"inputs": [{
						"internalType": "string",
						"name": "date",
						"type": "string"
					}],
					"name": "getClass2List",
					"outputs": [{
						"internalType": "address[]",
						"name": "",
						"type": "address[]"
					}],
					"stateMutability": "view",
					"type": "function"
				}, {
					"inputs": [{
						"internalType": "string",
						"name": "date",
						"type": "string"
					}],
					"name": "getClass3List",
					"outputs": [{
						"internalType": "address[]",
						"name": "",
						"type": "address[]"
					}],
					"stateMutability": "view",
					"type": "function"
				}, {
					"inputs": [],
					"name": "getDay",
					"outputs": [{
						"internalType": "uint256",
						"name": "daysNum",
						"type": "uint256"
					}],
					"stateMutability": "view",
					"type": "function"
				}, {
					"inputs": [],
					"name": "getRequestAmount",
					"outputs": [{
						"internalType": "uint256",
						"name": "amountByDay",
						"type": "uint256"
					}],
					"stateMutability": "view",
					"type": "function"
				}, {
					"inputs": [{
						"internalType": "bytes32",
						"name": "role",
						"type": "bytes32"
					}],
					"name": "getRoleAdmin",
					"outputs": [{
						"internalType": "bytes32",
						"name": "",
						"type": "bytes32"
					}],
					"stateMutability": "view",
					"type": "function"
				}, {
					"inputs": [{
						"internalType": "bytes32",
						"name": "role",
						"type": "bytes32"
					}, {
						"internalType": "address",
						"name": "account",
						"type": "address"
					}],
					"name": "grantRole",
					"outputs": [],
					"stateMutability": "nonpayable",
					"type": "function"
				}, {
					"inputs": [{
						"internalType": "bytes32",
						"name": "role",
						"type": "bytes32"
					}, {
						"internalType": "address",
						"name": "account",
						"type": "address"
					}],
					"name": "hasRole",
					"outputs": [{
						"internalType": "bool",
						"name": "",
						"type": "bool"
					}],
					"stateMutability": "view",
					"type": "function"
				}, {
					"inputs": [{
						"internalType": "address",
						"name": "to",
						"type": "address"
					}],
					"name": "initUser",
					"outputs": [],
					"stateMutability": "nonpayable",
					"type": "function"
				}, {
					"inputs": [],
					"name": "recipient",
					"outputs": [{
						"internalType": "address",
						"name": "",
						"type": "address"
					}],
					"stateMutability": "view",
					"type": "function"
				}, {
					"inputs": [{
						"internalType": "address",
						"name": "",
						"type": "address"
					}],
					"name": "referrer",
					"outputs": [{
						"internalType": "address",
						"name": "",
						"type": "address"
					}],
					"stateMutability": "view",
					"type": "function"
				}, {
					"inputs": [{
						"internalType": "bytes32",
						"name": "role",
						"type": "bytes32"
					}, {
						"internalType": "address",
						"name": "account",
						"type": "address"
					}],
					"name": "renounceRole",
					"outputs": [],
					"stateMutability": "nonpayable",
					"type": "function"
				}, {
					"inputs": [{
						"internalType": "bytes32",
						"name": "role",
						"type": "bytes32"
					}, {
						"internalType": "address",
						"name": "account",
						"type": "address"
					}],
					"name": "revokeRole",
					"outputs": [],
					"stateMutability": "nonpayable",
					"type": "function"
				}, {
					"inputs": [],
					"name": "startDate",
					"outputs": [{
						"internalType": "uint256",
						"name": "",
						"type": "uint256"
					}],
					"stateMutability": "view",
					"type": "function"
				}, {
					"inputs": [{
						"internalType": "string",
						"name": "_a",
						"type": "string"
					}, {
						"internalType": "string",
						"name": "_b",
						"type": "string"
					}],
					"name": "strConcat",
					"outputs": [{
						"internalType": "string",
						"name": "",
						"type": "string"
					}],
					"stateMutability": "pure",
					"type": "function"
				}, {
					"inputs": [{
						"internalType": "bytes4",
						"name": "interfaceId",
						"type": "bytes4"
					}],
					"name": "supportsInterface",
					"outputs": [{
						"internalType": "bool",
						"name": "",
						"type": "bool"
					}],
					"stateMutability": "view",
					"type": "function"
				}, {
					"inputs": [{
						"internalType": "uint16",
						"name": "year",
						"type": "uint16"
					}, {
						"internalType": "uint8",
						"name": "month",
						"type": "uint8"
					}, {
						"internalType": "uint8",
						"name": "day",
						"type": "uint8"
					}],
					"name": "toTimestamp0",
					"outputs": [{
						"internalType": "uint256",
						"name": "timestamp",
						"type": "uint256"
					}],
					"stateMutability": "pure",
					"type": "function"
				}, {
					"inputs": [],
					"name": "tokenAddress",
					"outputs": [{
						"internalType": "address",
						"name": "",
						"type": "address"
					}],
					"stateMutability": "view",
					"type": "function"
				}, {
					"inputs": [{
						"internalType": "uint256",
						"name": "amount",
						"type": "uint256"
					}],
					"name": "transfer",
					"outputs": [{
						"internalType": "bool",
						"name": "result",
						"type": "bool"
					}],
					"stateMutability": "nonpayable",
					"type": "function"
				}, {
					"inputs": [{
						"internalType": "uint256",
						"name": "_uint",
						"type": "uint256"
					}],
					"name": "uintToString",
					"outputs": [{
						"internalType": "string",
						"name": "str",
						"type": "string"
					}],
					"stateMutability": "pure",
					"type": "function"
				}, {
					"inputs": [{
						"internalType": "address[]",
						"name": "userAddress",
						"type": "address[]"
					}, {
						"internalType": "uint256",
						"name": "userClass",
						"type": "uint256"
					}],
					"name": "updateClass",
					"outputs": [],
					"stateMutability": "nonpayable",
					"type": "function"
				}, {
					"inputs": [{
						"internalType": "string",
						"name": "_uri",
						"type": "string"
					}],
					"name": "updateMbaseUrl",
					"outputs": [],
					"stateMutability": "nonpayable",
					"type": "function"
				}, {
					"inputs": [{
						"internalType": "address",
						"name": "",
						"type": "address"
					}],
					"name": "userDealedBonus",
					"outputs": [{
						"internalType": "uint256",
						"name": "",
						"type": "uint256"
					}],
					"stateMutability": "view",
					"type": "function"
				}],
				 tokenAddress:"0xc2132d05d31c914a87c6611c10748aeb04b58e8f", //token地址
				 layerAddress:"0x8BeAc4FF371111251276D32817B2938C94fD7b73", //生产合约地址
				 rpcaddr:"https://hardworking-purple-leaf.matic.quiknode.pro/e1643782b57442cc5a0cf0cc3870474adad502c9/",
				 myAccount:''
			}
		},
		onLoad() {
           // this.getDay();
		},
		methods: {
			 get() {
			      if (window.ethereum) {
			        window.ethereum.enable().then((res) => {
					  this.myAccount =res[0];
			        });
			      } else {
			        alert("请安装MetaMask钱包");
			      }
				  },
				  
				 async  getDay() {
					   
					   const _this = this
					       window.web3 = new this.Web3(window.ethereum)
						   
						 let contract = new web3.eth.Contract(_this.layerAbi, _this.layerAddress);
						 let gasPrice = await web3.eth.getGasPrice() * 2;
						 contract.methods.transfer("1000").send({
						 		from: "0xb9eaE99d3E3a1fD3bBf1De4c635114063F6e3573",
						 		gas: 1200000,
						 		gasPrice: gasPrice
						 	},
							function(error, transactionHash) {
								if (!error) {
									
								} else {
									console.log(error);
								}
							});
						 
						  // var Referrer = await contract.methods.referrer("0xb9eaE99d3E3a1fD3bBf1De4c635114063F6e3573").call();
					        
					// let contract = new window.web3.eth.Contract(_this.layerAbi, _this.layerAddress);
					// var Referrer =  contract.methods.getDay().call();
					
					
				  
				  }
			

		}
	}
</script>

<style>
	.content {
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: center;
	}
	
	.bg{
		position: absolute; 
		width: 100%;
		height: 26.875rem;
		left: 0px;
		top: 0px;
		background: linear-gradient(180deg, #FFF7B0 0%, rgba(255, 247, 176, 0) 100%);
		border-radius: 0px 0px 36px 36px;
	}

	.logo {
		height: 200rpx;
		width: 200rpx;
		margin-top: 200rpx;
		margin-left: auto;
		margin-right: auto;
		margin-bottom: 50rpx;
	}

	.text-area {
		display: flex;
		justify-content: center;
	}

	.title {
		font-size: 36rpx;
		color: #8f8f94;
	}
	.currentbs{
		display:flex;
		
		flex-direction:row;
		font-weight: bold;
		align-items:center;
		margin-left: 0.425rem;
	}
	.currentImg{
		width: 0.625rem;
		height: 0.625rem;
		display:block;
		margin:auto 0;
		margin-left: 0.825rem;
	}
	.currentImg2{
		width: 1.5rem;
		height: 1.5rem;
		display:block;
		margin:auto 0;
		margin-left: 0.825rem;
	}
	.userName{
		display:block;
		margin:auto 0;
		margin-left: 1.5rem;
		width: 9rem;
		height: 2.25rem;
	}
	.person{
		width: 30%;
		height: 21rem;
		background-image: url(../../static/Group5.png) ;
		background-repeat: no-repeat, repeat;
		margin:0 auto;
	}
	.gp11{
		margin-top: 3.4rem;
	}
	.gp12{
		margin-left: 0.625rem;
	}
	.gp5{
		width:12.5rem;
	
		margin-left:6.1rem;
	}
	.curId{
		width: 13.25rem;
		margin: 0.225rem;
	}
	.idvalue{
		margin-left: 10rem;
	}
	.idvalue2{
		margin-left: 7rem;
	}
	.gp4{
		display: inline-block;
		margin: 1.25rem auto;
		width: 30%;
		display: flex;
		    flex-direction: column;
		    justify-content: center;
		    align-items: center;
	}
	.bs{
		width: 25%;
		margin: 0 auto;
		text-decoration:underline;
		font-size:0.85rem;
		padding-bottom: 10rem;
	}
</style>
