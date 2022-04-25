[по-русски](/README-ru.md)

## F12+ FarmersWorld.io tools by AngelFarmers
> Play like professional.
> Farm resources and participate in building the Metaverse.
> Join our AngelFarmers Guild, participate in DAO, invest and get dividends

![Снимок экрана 2022-03-02 в 21 02 57](https://user-images.githubusercontent.com/6615/156410626-00a41166-04fe-4112-987d-6a863e71dfc3.png)

F12+ is open source dapp that helps FarmersWorld.io players farm resources and trade on Atomic and Alcor.

https://fw.angelfarmers.com - official version for AngelFamers guild members


### Features overview:
1. Calculate current value of your farm assets
2. Estimate earnings and ROI
3. Automatically perform mundane actions like claiming, repairing, recovering energy, feeding animals and more
4. Easily perform farm management actions like Withdraw and deposit funds, Exchange tokens, Transfer NFTs and tokens, Craft and buy in the game market, Stake for CPU, Exchange crops, Sell NFTs on Atomic and etc.
5. Overview and manage multiple farms in one window. Calculate total value and estimate earnings on all your farms.
6. Use non-Wax Cloud Wallet (Anchor and others) accounts for farming
7. Check-in with your farms status on Telegram via F12+ bot. Get notifications for all transfers on your accounts and issues
8. Analyze Atomic market for artitrage opportunities
9. Analyze Alcor orderbooks for trading
10. Bilingual support in English and Russian

### About AngelFarmers
We are a gaming league of players and investors, enjoying [FarmersWorld.io](https://farmersworld.io) game on WAX blockchain. 
Our goal is to support fellow members of the league in playing the game, earning passive income and having most fun with it.
In order to help best players expand and investors make most of their money we have created a guid token - AWAX.

AWAX or Angel WAX is a savings/dividends/governance token of AngelFarmers Guild. AWAX is a native token on WAX blockchain that is traded on Alcor exchange:

[Swap WAX/AWAX](https://wax.alcor.exchange/swap?output=WAX-eosio.token&input=AWAX-awaxdaotoken)

[Orderbooks for WAX/AWAX](https://wax.alcor.exchange/trade/awax-awaxdaotoken_wax-eosio.token)

Every guild member who invests 5% of their income from Farmers World into AWAX are eligible to participate in the following:
1. Propose new features and work done for F12+ tools
2. Vote on new development and community agenda
3. Receive airdrops with NFTs and tokens earned by community investfund
4. Receive dividends from community investment fund
5. Receive funds to invest and trade from community fund
----

### Key settings:
In order to make the app work with Firestore Database you will need to create a new Firebase project, add a web app and generate API_KEY and obtain configuration info from Firebase.

#### for api keys----

login to google
Goto https://console.firebase.google.com 

obtain below 7 api details and fill the dots and save the file as as .keys.js inside angel-ui folder (on windows sometimes file name extension are hidden, to show it go to, file explorer view tick on file name extensions)

### Steps to get api keys in google firebase ->
1. Enter Your Project Name eg: f12ui then-> continue 
2. It will say in enable google analytics ok(for measurementId) -> continue 
3. create new firebase analytics project -> create project 
4. creating project take time (say your new project ready)-> continue 


5. Go to Firestore database (Left Menu 2nd no)-> create database
6. select closest regional server(find from gcping.com)-> select & Enable

Provisioning Cloud Firestore..

7. (Left Menu)Click gear icon(Project Overview)-> project settings
8. scroll down to "your apps"
9. then click </> (means web app)
10. fill your webapp name ->like f12ui ->register app
11. then copy the 7 api details inside "" and replace them eg.in top, and save as 
.keys.js

Place the .keys.js file inside angelfarmers-ui-main folder place as root

[google work done close the firebase tab no need for that]
---

Place the configuratino info into .keys.js file in the root project folder with the following code:

```
export const FB_APIKEY="..."
export const FB_authDomain="..."
export const FB_projectId="..."
export const FB_storageBucket="..."
export const FB_messagingSenderId="..."
export const FB_appId="..."
export const FB_measurementId="..."
```

### Installation 
Install node js (eg: 16.14.2 64bit) 
install 'chocolaty script' tick yes next (windows sdk etc. comes with node js, while installation(take time))

### Extract and CD to angel-ui folder (save angel-ui in desktop. use command prompt CMD)
```
cd angel-ui
```

### Install npm package manager.
```
npm install -g npm
```
If this shows error means there are new dependency avilable, (eg: "sass": "~1.32.0", "sass-loader": "^10",)

### Addition stuff
```
npm install -g node-gyp
```

### Install yarn package manager.
```
npm install -g yarn
```

----
### Use

#### Project setup
```
yarn install
```
Success install will download and install all the dependencies listed inside package.json to node_modules folder


#### Compiles and hot-reloads for development
```
yarn serve
```
App running in development (not optimed for final use)
  App running at:
  - Local:   http://localhost:8080/     
  - Network: http://192.168.xx.xx:8080/ (LAN Address)

open browser then check the localhost:8080 to see if it running okay its in development it is not optimised to use 
use ctrl C to cancel the app running in cmd(repeat ctrl c 2 3 times to stop it)

### Compiles and minifies for production
```
yarn build
```
To build for final use web ui app will be installed in dist folder


### To run the app in dist folder
```
npm install -g serve
```
(it will install the serve, -g means globle)
check with
```
serve --version
```

### Launch the app
```
serve dist
```
it will be optimised, you can open it on browser by localhost:3000 as mentioned
(if you want to close the app, close it with ctrl C. or
close the cmd window, after reboot if you do in future, to run this app open cmd as admin, cd to angelfarmers-ui-main folder type serve dist, it will be launched then you can open it on browser localhost with port no. )

---


## Contributions

Chineese translation by cnscdh!
