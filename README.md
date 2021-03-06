[![Build Status](https://travis-ci.org/cloudfoundry/tunnel-vmc-plugin.png)](https://travis-ci.org/cloudfoundry/tunnel-vmc-plugin)
[![Gem Version](https://badge.fury.io/rb/tunnel-vmc-plugin.png)](http://badge.fury.io/rb/tunnel-vmc-plugin)

## Deprecated
VMC and its plugins have been renamed. You can find the current version of the code for this gem at
http://github.com/cloudfoundry/tunnel-cf-plugin

## Tunnel
### Info
This plugin allows you to connect to a Cloud Foundry service using your own command line client. By default, the plugin supports *redis*, *mysql*, *mongodb*, and *postgresql*.

### Installation
```
gem install tunnel-vmc-plugin
```

### Usage
```
tunnel [INSTANCE] [CLIENT]        Create a local tunnel to a service.
```

You can add support for other command-line clients by providing a `~/.vmc/clients.yml` file with the following format:

```yaml
service_name:
  client_program_name: command line arguments
  client_program_name_2:
    command: command line arguments
    environment:
      - ENV_VAR_NAME=env_var_value
```
