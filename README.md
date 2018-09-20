# *EWASM Studio* for Remix

A lightweight development environment for eWASM.

The application is available in the `app` directory, all commands below must be done there.

## Installation
`npm install`

## Usage
`PORT=some_port_number npm start`

The default port (if not specified) is 3000.

* git clone remix-ide and checkout #1524 ethereum/remix-ide#1524

* git clone remix, checkout #973 ethereum/remix#973,

* in remix/remix-lib `npm install`, `npm link`, then `npm link remix-lib` in /remix-ide

* in remix/remix-solidity, `npm install`, `npm link`, then `npm link remix-solidity` in /remix-ide

* `npm install` in /remix-ide
Implemented:

* git clone ewasm-studio-remix https://github.com/oogetyboogety/ewasm-studio-remix

* `npm start` in /ewasm-studio-remix, `npm start` in /remix-ide, and start your geth node as illustrated here:
https://github.com/ewasm/testnet/

* load the plugin from the settings tab in remix-ide
`{ "title": "ewasm-studio-remix", "url": "http://127.0.0.1:3000" }`


* Paste a WAST into a new file, such as the basic ledger contract here:
https://github.com/ewasm/assemblyscript-ewasm-api
or
* use remixd to load a WAST file into Remix and open it

* Click the Get from remix button

* If you haven't checked out the new PRs, set a value and deploy the contract to testnet directly from the plugin

* If you have checked out the latest PRs, click the Send to remix button and Deploy from the Run tab

* Call the functions fallback function with some arbitrary value using JSON inputs to the `fallback` function
