# Tron-Box
Tronbox User Guide
## Installation
`$ npm install -g tronbox`
## OS requirement
- NodeJS 5.0+
- Windows, Linux, or Mac OS X

## Features
1. Initialize a Customer Tron-Box Project<br>
`$ tronbox init`
<br>

2. Download a Dapp, ex: metacoin-box<br>
`$ tronbox unbox metacoin`
<br>

3. Contract Compiler<br>
`$ tronbox compile`
<br>
  To compile for all contracts, select --compile-all. <br>
`$ tronbox compile --compile—all`
<br>
Optionally, you can select:<br>
--compile-all: Force compile all contracts. <br>
--network save results to a specifict hose network<br>
<br>

## 4. Contract Migration<br>
`$ tronbox migrate`
<br>
This command will make all migrations    . If your previous migration was successful, `tronbox migrate` will invoke a newly created migration. If there is no new migration script, this command    Instead, you can use `--reset` to start over the migration script. 
`$ tronbox migrate --reset` 
<br>
## 5. Start Console<br>
This will use the default network to start a console. It will automatically connect to a TVM client. You can use `--network` to change this. 
<br>
$ tronbox console
<br>
supports tronbox command, EX: migrate --reset === tronbox migrate --reset
<br>
## Extra Feature:<br>
1）all compiled contract can be used same as develop and testing in the front-end<br>
2）for each command, your contract will be re-loaded. <br> after using migrate --reset, you can use the new address andd binary code<br>
3）promiss will automatically be logged dont have to use extra then command<br>
<br>
6、testing<br>
$ tronbox test<br>
for specific file：<br>
$ tronbox test ./path/to/test/file.js<br>
