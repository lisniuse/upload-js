# upload-js

A lightweight AJAX upload library.

## Usage

### import

```javascript
import upload from 'upload-js';
// or:
const upload = require('upload-js');
```

### case

```javascript
import upload from 'upload-js';

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
