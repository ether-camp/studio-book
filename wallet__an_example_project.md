# Example projects


Out of the box, Studio has a very basic [example project](https://github.com/ether-camp/default-ws/tree/master/example-project) you can copy to a new project folder and edit to get going on your project. Example app demonstrates working with Ethereum from javascript using web3.js and ethereumjs-tx. Edit the web/src/app.js to check the web3 JSON RPC url.

Or you can study the Wallet app example which is more complete.  In the terminal type: 

```
cd ~/workspace 
git clone https://github.com/ether-camp/wallet.git``` 
  
Which loads a copy of the Wallet.app [1] into your workspace directory:


![](Ether-Camp-dir1.png)

The app directory [2] with app.js [3], the main application javascript file. The______ file must be edited to ensure running sandbox and javascript files are pointed to the correct ports. Ethereum.json is your Sandbox configuration file you can edit to change addresses, balance etc.. .

The wallet app uses [Browserfy and Gulp](https://www.viget.com/articles/gulp-browserify-starter-faq) for compile and dependency package management. However, **with Ethereum Studio, you are free to use whatever framework you choose.**



