# Running your app

Once you have sandbox running you can run your app. But,** first configure your app.js correctly**. You need to make sure your app has the correct JSON-RPC URL of your sandbox (or livenet node). In the example /workspace/example-project/web/app.js file, edit the lines.

## 



**Set the correct SandboxID#:**

```var sandboxId = '[somenumber]';```

change to

```var sandboxId = '[your_running_sandboxID#]';```


## 



**AND**


## 



**Set the correct Sandbox URL:**

```var url = 'https://' + window.location.hostname + ':8555/sandbox/' + sandboxId;```

change to

```var url = 'https://[your_username].by.ether.camp:8555/sandbox/' + sandboxId;```


## 



**Check and edit your ABI as needed**

In the /workspace/example-project/web/app.js file has a Array definition ABI =[ ....  ]
Remember to check that its content corresponds to the ABI json in the sandbox (or livenet) contract address you deployed (see Sandbox panel section).




