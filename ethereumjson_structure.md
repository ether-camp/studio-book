# ethereum.json 
(updated fir new sol 0.4 and IDE)

This file is at the root of your project folder to ensure Sandbox runs with pre funded accounts addresses. If you start a new project, make sure you have an ethereum.json file in place:

**NEW update: Note** ```  "deploy": ["Contract"],```  in the ethereum.json file. This is where you list the contract(s), in your project contract folder, you want deployed. If nothing is listed, all contracts in the project contract folder will be deployed when you select 'run all contracts' in the IDE.

Below is a complete ethereum.json file for the example project:
```
//your list of contracts
{
  "contracts": "contracts",
  
  "deploy": ["Contract"],
  
  "env": {
    "block": {
      "coinbase" : "0x2adc25665018aa1fe0e6bc666dac8fc2697ff9ba",
      "difficulty" : "0x0100",
      "gasLimit" : 3141592,
      "gasPrice": 60000000000
    },
    "accounts": {
      "0xdedb49385ad5b94a16f236a6890cf9e0b1e30392": {
        "balance": 1000000000000000000000000000000000000000000000000000000 ,
        "nonce": "0x1cf",
        "pkey": "0x974f963ee4571e86e5f9bc3b493e453db9c15e5bd19829a4ef9a790de0da0015", 
        "default": true
      },
      "0xcd2a3d9f938e13cd947ec05abc7fe734df8dd826": {
        "balance": "0x1000000000000000000000000000000000000",
        "nonce": "1430",
        "pkey": "cow",
        "default": false,
        "storage": {
          "0x0f": 200010,
          "0x01": "0x200001"
        }
      },
      "0x084f6a99003dae6d3906664fdbf43dd09930d0e3": {
        "balance": 1234567890123345,
        "deploy": {
          "source": "_pre/name_reg.sol",
          "contract": "NameReg"
        }
      }
    }
  }
}
```

