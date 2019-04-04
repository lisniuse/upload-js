# Uploadman

A lightweight AJAX upload library.

## Installation

This is a [Node.js](https://nodejs.org/en/) module available through the
[npm registry](https://www.npmjs.com/).

Before installing, [download and install Node.js](https://nodejs.org/en/download/).
Node.js 8.0 or higher is required.

Installation is done using the
[`npm install` command](https://docs.npmjs.com/getting-started/installing-npm-packages-locally):

```bash
$ npm install uploadman
```

## Usage

### import

```javascript
import upload from 'uploadman';
// or:
const upload = require('uploadman');
```

### case

```javascript
import upload from 'uploadman';

const options = {
  headers: Object,
  withCredentials: Boolean,
  file: Object,
  data: Object,
  filename: String,
  action: String,
  onProgress: e => {
    console.log(~~e.percent);
  },
  onSuccess: res => {
    console.log('success');
  },
  onError: err => {
    console.log('error');
  }
};
upload(options);
```
