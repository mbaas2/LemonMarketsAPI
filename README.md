# LemonMarketsAPI

This is a APL SDK for accessing the Lemon Markets API. API documentation can be found here: [https://docs.lemon.markets/](https://docs.lemon.markets/)

lemon.markets is in closed beta and this SDK is a work in progress. Pull requests to expand the SDK or improve its reliability are welcomed.

## Which APL?

This SDK is implemented using Dyalog APL 18.2 and it will probably not work with lower versions. (If you absolutely need it for an earlier version,
let me [know](./issues)!)
If you want to use other dialects, feel free to use this code as your v1, but I intend to only support the Dyalog implementation.

## Installation
First, clone this repository to your local machine.

git clone https://github.com/mbaas2/LemonMarketsAPI.git

Then `]LOAD` the .aplc (or `]LINK` the folder you'ver cloned into)

## Configuration

Before running the code, you obviously need to have access to LemonMarkets and you'll need a personal API Key. (Get it from LM's dashboard)
Store this API Key either in the .json5 config file or (preferred) in an environment variable (or a .dcfg config file)
## Usage

Run `LemonMarkets_API.test` to execute basic tests.

## More

This isn't done yet - I'm still experimenting & adding to it. Feel free to help with Pull Requests
or create Issues if you find any bugs or want enhancements.