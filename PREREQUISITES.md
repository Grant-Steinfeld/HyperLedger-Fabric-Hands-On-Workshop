# Installation and Requirements for for setting up the IBM Blockchain Platform Extension for Visual Studio Code


The IBM Blockchain Platform extension for VS Code, helps developers to create, test and debug smart contracts, connect to Hyperledger Fabric environments, and build applications that transact on your blockchain network.

For a step-by-step guide on getting started with the extension's features, access 
our Beginner Tutorial via our integrated Home page. Alternatively, explore, clone and open the Hyperledger Fabric samples, all without leaving VS Code. For more comprehensive documentation, [follow this link](https://cloud.ibm.com/docs/services/blockchain/howto?topic=blockchain-develop-vscode)



## Installation

Please visit the [Visual Studio Code Marketplace](https://marketplace.visualstudio.com/items?itemName=IBMBlockchain.ibm-blockchain-platform) for installation and more details.

## Requirements

We strongly suggest you setup Node Version Manager (nvm) as it allows you to install and run different versions of node and npm on your computer.  This is very useful, especially as the node version requirements and it's dependancies are often version dependant.

At this time of writing ( Oct 19th 2019 ) simply run

``` sh
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.35.0/install.sh | bash
echo "follow instructions to reload your shell to run nvm"
```

**If installing Node and npm using a manager such as 'nvm', you will need to set the default/global version and restart VS Code for the version to be detected by the IBM Blockhain Platform Extension Prerequisites page.**


You will need the following installed in order to use the extension:
- Windows 10, Linux, or Mac OS are currently the supported operating systems.
- [VS Code version 1.32 or greater](https://code.visualstudio.com) - ( at this time of writing I have 1.39.2 on Mojave/MacOS )
- [Docker version v17.06.2-ce or greater](https://www.docker.com/get-docker)
- [Docker Compose v1.14.0 or greater](https://docs.docker.com/compose/install/)
- [Node v8.x or v10.x and npm v6.x or greater](https://nodejs.org/en/download/)


If you are using Windows, you must also ensure the following:
- You are using Windows 10 Pro or Enterprise and have the Anniversary Update 1607
- Docker for Windows is configured to use Linux containers (this is the default)
- You have installed the C++ Build Tools for Windows from [windows-build-tools](https://github.com/felixrieseberg/windows-build-tools#windows-build-tools)
- You have installed OpenSSL v1.0.2 if using Node 8, or v1.1.1 if using Node 10 from [Win32 OpenSSL](http://slproweb.com/products/Win32OpenSSL.html)
  - Install the normal version, not the version marked as "light"
  - Install the Win32 version into `C:\OpenSSL-Win32` on 32-bit systems
  - Install the Win64 version into `C:\OpenSSL-Win64` on 64-bit systems

You can check your installed versions by running the following commands from a terminal:
```sh
node --version
npm --version
docker --version
docker-compose --version
```

you should see something similar to the following output:

``` sh
/tmp node --version
v10.16.3
/tmp npm --version
6.11.3
/tmp docker --version
Docker version 19.03.2, build 6a30dfc
/tmp docker-compose --version
docker-compose version 1.24.1, build 4667896b
```


