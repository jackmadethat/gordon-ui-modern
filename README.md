# Gordon-UI for the Modern Toolchain

## About

This repo is my attempt at updating the excellent Gordon-UI for the modern toolchain without using Docker or modifying the core code/functionality. Tested working with Windows 10. As it relies on older and deprecated packages, stability is not a guarantee.

## Links
- [Gekko Trading Bot](https://github.com/askmike/gekko)
- [Gekko Quasar UI](https://github.com/H256/gekko-quasar-ui)

## Required Environment

This repo *will not work* with any other versions than these:

```
quasar -v
1.9.6
```
```
npm -v
11.12.1
```
```
node -v
v24.15.0
```

## Setup

1. Start your Gekko Instance as normal with `node gekko --ui`

2. Clone this repo to a new directory

3. CD into the cloned repo

4. Install/Tweak packages

```
npm remove node-sass babel-core babel-preset-env babel-loader
```
```
npm install sass sass-loader@10.5.2 @babel/core @babel/preset-env babel-loader@8 babel-core@7.0.0-bridge.0 --save-dev
```
```
npm remove vue vue-template-compiler
```
```
npm install vue@2.6.14 vue-template-compiler@2.6.14 --save
```
```
npm install -g @quasar/cli
```
```
npm install webpack-dev-server@3.11.3 sockjs-client@1.5.2 websocket-driver@0.7.4 --save-dev
```
5. Install

```
npm run build
```
6. Run

```
npm run dev
```
7. A browser tab should open with the Gordon-UI frontend. If not, navigate to `http://localhost:8080`

## Screenshots

![image1](img/gekko-quasar-1.png?raw=true "Screenshot 1")
![image2](img/gekko-quasar-2.png?raw=true "Screenshot 2")
![image3](img/gekko-quasar-3.png?raw=true "Screenshot 3")
![image4](img/gekko-quasar-4.png?raw=true "Screenshot 4")
![image5](img/gekko-quasar-5.png?raw=true "Screenshot 5")
![image6](img/gekko-quasar-6.png?raw=true "Screenshot 6")
![image7](img/gekko-quasar-7.png?raw=true "Screenshot 7")
![image8](img/gekko-quasar-8.png?raw=true "Screenshot 8")
![image9](img/gekko-quasar-9.png?raw=true "Screenshot 9")

