# *EWASM Studio* for Remix

A lightweight development environment for eWASM.

The application is available in the `app` directory, all commands below must be done there.

## Installation
`npm install`

## Usage
`PORT=some_port_number npm start`

The default port (if not specified) is 3000.

* load the plugin from the settings tab in remix-ide
`{ "title": "ewasm-studio-remix", "url": "http://127.0.0.1:3000" }`


* Paste a WAST into a new file, such as the basic ledger contract here:
https://github.com/ewasm/assemblyscript-ewasm-api
or
* use remixd to load a WAST file into Remix and open it

* Click the Get from remix button

* If you are not on Remix alpha, set a value and deploy the contract to testnet directly from the plugin

* If you are on Remix alpha ([here](https://remix-alpha.ethereum.org/ or `npm-install remix-ide`), click the Compile button and Deploy from the Run tab

* Call the functions fallback function with some arbitrary value using hex string input prefixed with 'raw:0x...' to the `fallback` function
