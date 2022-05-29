# LemonMarketsAPI

This is a APL SDK for accessing the Lemon Markets API. API documentation can be found here: [https://docs.lemon.markets/](https://docs.lemon.markets/)

lemon.markets is in closed beta and this SDK is a work in progress. Pull requests to expand the SDK or improve its reliability are welcome.

## Which APL?

This SDK is implemented using [Dyalog APL](https://dyalog.com) [18.2](https://www.dyalog.com/dyalog/dyalog-versions/182.htm) and it will probably not work with lower versions. (If you absolutely need it for an earlier version,
let me [know](./issues)!)
If you want to use other dialects, feel free to use this code as your v1, but I intend to only support the Dyalog implementation.

## Installation

First, clone this repository to your local machine.

git clone https://github.com/mbaas2/LemonMarketsAPI.git

Then `]LOAD` the .aplc (or `]LINK` the folder you've cloned into)

## Configuration

Before running the code, you obviously need to have access to LemonMarkets and you'll need a personal API Key. (Get it from LM's dashboard)
Store the API Key either in the .json5 config file in param `APIKey` or (preferred) in an environment variable (or a .dcfg config file) called `LemonMarkets_APIKEY`.
In the same way, your PIN is searched for using name `LemonMarkets_PIN`  (in env or .dcfg) or just ` PIN`  in the .json5-file.

## Usage

Run `LemonMarkets_API.test` to execute basic tests.

## Currently implemented endpoints

We assume "knowledgeable users", so there's not much care taken to handle error messages.
I'm planning to change this before calling it "final", but currently you basically
get what you asked for ;)

Lemon Market's API has two major entry points:
* Trading
* Market

And this kit is structured identically. Once you instantiated the class, you get acccess to vars `Market`
and `Trading` that expose the endpoints.

### Trading

* withdrawal

### Market

* instruments
* trades
* quotes

The argument of those fns is an empty string or query-params otherwise.

## More

This isn't done yet - I'm still experimenting & adding to it. Feel free to help with Pull Requests
or create Issues if you find any bugs or want enhancements.
