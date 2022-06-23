# nodejs-ectoken
> _node.js implementation of Edgio token (`ectoken`)_

## Table of Contents

- [Background](#background)
- [Install](#install)
- [Usage](#usage)
- [Example](#example)
- [Contribute](#contribute)
- [License](#license)

## Background

node.js implementation of the "Edgio Token" (`ectoken`) -see main repo [ectoken](https://github.com/edgioinc/ectoken) for more details.

# Install
```
npm install ectoken
```

## Usage
* **encrypt**(key, params, verbose)
* **decrypt**(key, token, verbose)

## Example
```javascript
const ectoken = require('ectoken').V3;

// encrypt
const token = ectoken.encrypt('keyvalue', 'ec_expire=1257642471&ec_clientip=11.22.33.1');

// decrypt
const params = ectoken.decrypt('keyvalue', token);
```

## Contribute
We welcome issues, questions and pull requests.

## License
This project is licensed under the terms of the Apache 2.0 open source license. Please refer to the `LICENSE` file for the full terms.