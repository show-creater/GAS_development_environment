# GAS Development Environment
This repository provides a streamlined development environment for Google Apps Script (GAS) projects using clasp and rollup. It is designed to facilitate local development, efficient bundling, and deployment to the GAS platform.

## Features
* Local Development: Write, edit, and organize your GAS scripts locally using modern development tools.
* Rollup Integration: Bundle your scripts efficiently, enabling the use of ES modules and other modern JavaScript features.
* TypeScript Support: Fully supports TypeScript for type safety and improved development experience.
* Clasp Deployment: Seamless deployment to Google Apps Script via the clasp CLI.
## Requirements
* Node.js (version 16 or later)
* Google account with access to Apps Script
## Installation
1. Clone this repository:

```bash
git clone https://github.com/show-creater/GAS_development_environment.git
cd GAS_development_environment
```

2. Install dependencies:

```bash
npm install
```

3. Authenticate with clasp:

```bash
clasp login
```

## Usage
### Local Development
1. Write your code in the src directory.
2. Use modern JavaScript/TypeScript features as needed.
### Build and Deploy
1. Bundle your scripts with Rollup:

```bash
npm run build
```
This compiles and bundles your code into the dist directory.

2. Push your changes to Apps Script:

```bash
clasp push
```
Test your scripts in the Apps Script editor or directly in your project.

## Scripts
* `npm run build`: Bundles the code using Rollup.
* `npm run deploy`: Builds and deploys the code to Apps Script.
* `clasp pull`: Pulls the latest changes from Apps Script.
* `clasp push`: Pushes local changes to Apps Script.
## Directory Structure
```plaintext
GAS_development_environment/
├── src/               # Source code directory
├── dist/              # Compiled and bundled files (generated by Rollup)
├── .clasp.json        # Clasp configuration
├── rollup.config.js   # Rollup configuration file
├── package.json       # Node.js dependencies and scripts
├── tsconfig.json      # TypeScript configuration file
└── README.md          # Project documentation
```

please check my [techblog](https://zenn.dev/ritsumei_arupak/articles/522af3c807416a)!
