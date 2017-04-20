# proxy\_env

## Installation
Clone this repository and run install.sh.

``` sh
$ git clone https://github.com/OUDON/proxy\_env ~/.proxy\_env
$ cd ~/.proxy\_env
$ ./install.sh
```
Add the following to your .bash\_profile.

``` sh
if [ -z "$PROXY_ENV_ROOT" ]; then
  export PROXY_ENV_ROOT=$HOME/util/proxy_env
fi
eval "$(proxy_env init)"
```

## Usage
Add proxy config.

``` sh
$ proxy_env add <PROXY_NAME> http://proxy.example.com:port
```

Set the proxy.

``` sh
$ proxy_env set <PROXY_NAME>
```

Show added proxies.

``` sh
$ proxy_env lis
```

## License
This software is released under MIT license.  
(c) 2017 OUDON.

