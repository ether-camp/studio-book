# Running your app

Once you have sandbox running you can run your app. But,** first configure some things correctly**. Here below is the checklist for running the example project. To set up and run your own dapps you can use this sample as a starting point and/or configure your own contract folder and[ ethereum.json](https://nogo10.gitbooks.io/ether-camp-live-studio-primer/content/ethereumjson_structure.html) to create your own sandbox runtime.

![](Ether-Camp-run-app.png)

You need to make sure your app has the correct JSON-RPC URL of your sandbox (or livenet node). In the example /workspace/example-project/web/app.js file, edit the lines.

## 




[1] **Set the correct SandboxID#:**

```var sandboxId = '[somenumber]';
var url = 'http://' + window.location.hostname + ':8555/sandbox/' + sandboxId;
var web3 = new Web3(new Web3.providers.HttpProvider(url));```

change to

```var sandboxId = '[your_running_sandboxID#]';
var url = 'https://[username].by.ether.camp:8555/sandbox/' + sandboxId;
var web3 = new Web3(new Web3.providers.HttpProvider(url));```


## 



**AND in line below**


## 



**Set the correct Sandbox URL:**

```var url = 'https://' + window.location.hostname + ':8555/sandbox/' + sandboxId;```

change to

```var url = 'https://[your_username].by.ether.camp:8555/sandbox/' + sandboxId;```


## 



**Check and edit your ABI as needed**

In the /workspace/example-project/web/app.js file has a Array definition ABI =[ ....  ]
Remember to check that its content corresponds to the ABI json in the sandbox (or livenet) contract address you deployed (see Sandbox panel section).

**Check your contract addresses**
[4] If your app refers to specific contracts running the sandbox, check the addresses listed in your app.

### Get Ethereum Studio ready:
![](Ether-Camp-run-app.png)

If you want to run a specific javascript file then see item [2] and [3] change your current directory to the project folder you want to run. Click the CWD (Change Working Directory) button and pick the project directory. Clear item [3].

For development and production the example-project is configured for :

Building:
```
$ npm install gulp-cli -g
$ npm install
$ gulp
```

Testing:
```
$ gulp test
```

Running:
```
$ cd web
$ npm install http-server -g
$ http-server
```