# IOTA Packager

This packager will compile the app into executables for Linux, MacOS and Windows...

## Prerequisites

1. Download [NodeJS](https://nodejs.org/en/download/)

2. Install [Electron](http://electron.atom.io):

  ```
  npm install -g electron-prebuilt
  ```

3. Install [Bower](https://bower.io/):

  ```
  npm install -g bower
  ```

4. Install [Electron Builder](https://github.com/electron-userland/electron-builder)

Electron Builder is used behind the scenes. Read their [instructions](https://github.com/electron-userland/electron-builder/wiki/Multi-Platform-Build) on how to set up your system.

## Instructions

1. Clone repository:

  ```
  git clone https://github.com/iotaledger/wallet-packager
  ```

2. Go to the `wallet-packager` directory:

  ```
  cd wallet-packager
  ```

3. Install other repo's:

  ```
  git clone https://github.com/iotaledger/wallet
  git clone https://github.com/iotaledger/iri
  ```

  Note: iri project does not exist yet -- make an IRI directory manually and place IRI.jar in it.

4. Install components

  ```
  npm install
  ```

5. Build package:

  ```
  npm run dist
  ```

  If you'd like to create a package only for a specific OS, you can do so like this: 

  ```
  npm run dist:win
  npm run dist:mac
  npm run dist:lin
  ```