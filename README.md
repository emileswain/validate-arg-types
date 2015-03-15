ValidateArgs
============


Simple validator to test, log and or throw errors.

## Installation

  npm install https://github.com/emileswain/simple-validator/tarball/master --save

  Not sure if there are more Calculator apps or Argument validators. So I won't pollute npm.
  

## Usage
```
  var ValidateArgs = require('validateargs');
  
  var validator = ValidateArgs('identifier');
  
  validator.throwThem().isString('isAString');
  
  validator.throwThem(false).isString('isAString').log();
  
  validator.isString('isAString').log().throw();
  
  
  validator.throwThem()
    .isString('a-string-value')
    .isNumber('a-number',1234)
    .isArray('a-array',[]);
```


## Contributing

I'm no javascript expert, writing this was in part a foray into writing an npm module on a whim.

## Thanks to 
https://quickleft.com/blog/creating-and-publishing-a-node-js-module/


## Release History

* 0.1.0 Initial release