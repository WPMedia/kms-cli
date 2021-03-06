#  [![NPM version][npm-image]][npm-url] [![Build Status][travis-image]][travis-url] [![Dependency Status][daviddm-image]][daviddm-url]

>  Command-line client for AWS KMS


## Install as nodejs module (global)

```
$ npm install kms-cli -g
```
## Install as a docker executable container
Please see this project: https://github.com/ddffx/docker-kms-cli

## Setup Environment variables

Pick the AWS Region your KMS key is accessible in, and export your Access Key ID and Secret Access Keys as environment variables for the script to work.  Get those secrets off the AWS console.

```
export AWS_REGION=us-east-1
export AWS_ACCESS_KEY_ID=<your access key id>
export AWS_SECRET_ACCESS_KEY=<your secret access key id>
```

## Usage

```
$ kms-cli --help
```
### Implemented Features

#### Encrypt
```
kms-cli encrypt -k my_kms_key_id --pt 'My plain text'
```
#### Decrypt
```
kms-cli decrypt  --ct 'My encrypted cipher text'
```
#### Describe Key
```
kms-cli describe  -k my_kms_key_id
```
## License

MIT © [Deb Das]()


[npm-image]: https://badge.fury.io/js/kms-cli.svg
[npm-url]: https://npmjs.org/package/kms-cli
[travis-image]: https://travis-ci.org/ddffx/kms-cli.svg?branch=master
[travis-url]: https://travis-ci.org/ddffx/kms-cli
[daviddm-image]: https://david-dm.org/ddffx/kms-cli.svg?theme=shields.io
[daviddm-url]: https://david-dm.org/ddffx/kms-cli
