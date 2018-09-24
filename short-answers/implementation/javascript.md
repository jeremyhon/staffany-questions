# Javascript/ES6 (10-15 mins)

1. Name the most commonly used Javascript Transpiler/Compiler in use today.
2. The following is some transpiled ES5 code. Transform it to ES8 code. Also give the answer to the last line of code.

```
    "use strict"

    var forEach = require('lodash/forEach');

    var sentence = "this is a very l0ng sentence";

    var findNumber = function findNumber(phrase) {
      var idx = -1;
      forEach(phrase ,function (char, index) {
        if (isNumber(char)) {
          idx = index;
        }
      });
      return idx;
    };

    var isNumber = function isNumber(c) {
      return '0123456789'.indexOf(c) !== -1;
    };

    console.log(findNumber(sentence));
```

3. Convert the following callback style code to async/await and promise style.

```
    import {fetchObjectAsync, fetchObjectPromise} from './api'
    import {hydrateAsync, hydratePromise} from './hydrate'
    import {encryptAsync, encryptPromise} from './encrypt'
    import {storeResult, storeResultPromise} from './store'

    fetchObjectAsync("/endpoint", (arrayData) => {
      let objectData = {}
      arrayData.forEach((element, idx) => {
        return hydrateAsync(element, hydrated => {
          Object.assign(objectData, {[idx]: hydrated})
          encryptAsync(objectData, (encrypted) => {
            return storeResult(encrypted)
          }
        })
      })
    })
```
