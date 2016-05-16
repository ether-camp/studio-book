# Running your app

Once you have sandbox running you can run your app. But,** before running your app.js , it must be configured correctly**. You need to make sure your app has the URL of your sandbox (or livenet node). In the example app.js file, edit the lines

Set the correct SandboxID#:
```var sandboxId = '80ea8ad42c';```
to
```var sandboxId = '[your_running_sandboxID#]';```


AND

Set the correct Sandbox URL:
```var url = 'https://' + window.location.hostname + ':8555/sandbox/' + sandboxId;```
to
```var url = 'https://[username].by.ether.camp:8555/sandbox/' + sandboxId;```

