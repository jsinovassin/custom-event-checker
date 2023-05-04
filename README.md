custom-event-checker
=================

jCustomer events checker CLI

[![oclif](https://img.shields.io/badge/cli-oclif-brightgreen.svg)](https://oclif.io)
[![Version](https://img.shields.io/npm/v/oclif-hello-world.svg)](https://npmjs.org/package/oclif-hello-world)
[![License](https://img.shields.io/npm/l/oclif-hello-world.svg)](https://github.com/oclif/hello-world/blob/main/package.json)

<!-- toc -->
* [Usage](#usage)
* [Commands](#commands)
<!-- tocstop -->
# Usage
<!-- usage -->
```sh-session
$ npm install -g custom-event-checker
$ custom-event-checker COMMAND
running command...
$ custom-event-checker (--version)
custom-event-checker/0.1.0 darwin-x64 node-v19.4.0
$ custom-event-checker --help [COMMAND]
USAGE
  $ custom-event-checker COMMAND
...
```
<!-- usagestop -->
# Commands
<!-- commands -->
* [`custom-event-checker help [COMMANDS]`](#custom-event-checker-help-commands)
* [`custom-event-checker plugins`](#custom-event-checker-plugins)
* [`custom-event-checker plugins:install PLUGIN...`](#custom-event-checker-pluginsinstall-plugin)
* [`custom-event-checker plugins:inspect PLUGIN...`](#custom-event-checker-pluginsinspect-plugin)
* [`custom-event-checker plugins:install PLUGIN...`](#custom-event-checker-pluginsinstall-plugin-1)
* [`custom-event-checker plugins:link PLUGIN`](#custom-event-checker-pluginslink-plugin)
* [`custom-event-checker plugins:uninstall PLUGIN...`](#custom-event-checker-pluginsuninstall-plugin)
* [`custom-event-checker plugins:uninstall PLUGIN...`](#custom-event-checker-pluginsuninstall-plugin-1)
* [`custom-event-checker plugins:uninstall PLUGIN...`](#custom-event-checker-pluginsuninstall-plugin-2)
* [`custom-event-checker plugins update`](#custom-event-checker-plugins-update)
* [`custom-event-checker validateEvents`](#custom-event-checker-validateevents)

## `custom-event-checker help [COMMANDS]`

Display help for custom-event-checker.

```
USAGE
  $ custom-event-checker help [COMMANDS] [-n]

ARGUMENTS
  COMMANDS  Command to show help for.

FLAGS
  -n, --nested-commands  Include all nested commands in the output.

DESCRIPTION
  Display help for custom-event-checker.
```

_See code: [@oclif/plugin-help](https://github.com/oclif/plugin-help/blob/v5.2.9/src/commands/help.ts)_

## `custom-event-checker plugins`

List installed plugins.

```
USAGE
  $ custom-event-checker plugins [--core]

FLAGS
  --core  Show core plugins.

DESCRIPTION
  List installed plugins.

EXAMPLES
  $ custom-event-checker plugins
```

_See code: [@oclif/plugin-plugins](https://github.com/oclif/plugin-plugins/blob/v2.4.7/src/commands/plugins/index.ts)_

## `custom-event-checker plugins:install PLUGIN...`

Installs a plugin into the CLI.

```
USAGE
  $ custom-event-checker plugins:install PLUGIN...

ARGUMENTS
  PLUGIN  Plugin to install.

FLAGS
  -f, --force    Run yarn install with force flag.
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Installs a plugin into the CLI.
  Can be installed from npm or a git url.

  Installation of a user-installed plugin will override a core plugin.

  e.g. If you have a core plugin that has a 'hello' command, installing a user-installed plugin with a 'hello' command
  will override the core plugin implementation. This is useful if a user needs to update core plugin functionality in
  the CLI without the need to patch and update the whole CLI.


ALIASES
  $ custom-event-checker plugins add

EXAMPLES
  $ custom-event-checker plugins:install myplugin 

  $ custom-event-checker plugins:install https://github.com/someuser/someplugin

  $ custom-event-checker plugins:install someuser/someplugin
```

## `custom-event-checker plugins:inspect PLUGIN...`

Displays installation properties of a plugin.

```
USAGE
  $ custom-event-checker plugins:inspect PLUGIN...

ARGUMENTS
  PLUGIN  [default: .] Plugin to inspect.

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

GLOBAL FLAGS
  --json  Format output as json.

DESCRIPTION
  Displays installation properties of a plugin.

EXAMPLES
  $ custom-event-checker plugins:inspect myplugin
```

## `custom-event-checker plugins:install PLUGIN...`

Installs a plugin into the CLI.

```
USAGE
  $ custom-event-checker plugins:install PLUGIN...

ARGUMENTS
  PLUGIN  Plugin to install.

FLAGS
  -f, --force    Run yarn install with force flag.
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Installs a plugin into the CLI.
  Can be installed from npm or a git url.

  Installation of a user-installed plugin will override a core plugin.

  e.g. If you have a core plugin that has a 'hello' command, installing a user-installed plugin with a 'hello' command
  will override the core plugin implementation. This is useful if a user needs to update core plugin functionality in
  the CLI without the need to patch and update the whole CLI.


ALIASES
  $ custom-event-checker plugins add

EXAMPLES
  $ custom-event-checker plugins:install myplugin 

  $ custom-event-checker plugins:install https://github.com/someuser/someplugin

  $ custom-event-checker plugins:install someuser/someplugin
```

## `custom-event-checker plugins:link PLUGIN`

Links a plugin into the CLI for development.

```
USAGE
  $ custom-event-checker plugins:link PLUGIN

ARGUMENTS
  PATH  [default: .] path to plugin

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Links a plugin into the CLI for development.
  Installation of a linked plugin will override a user-installed or core plugin.

  e.g. If you have a user-installed or core plugin that has a 'hello' command, installing a linked plugin with a 'hello'
  command will override the user-installed or core plugin implementation. This is useful for development work.


EXAMPLES
  $ custom-event-checker plugins:link myplugin
```

## `custom-event-checker plugins:uninstall PLUGIN...`

Removes a plugin from the CLI.

```
USAGE
  $ custom-event-checker plugins:uninstall PLUGIN...

ARGUMENTS
  PLUGIN  plugin to uninstall

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Removes a plugin from the CLI.

ALIASES
  $ custom-event-checker plugins unlink
  $ custom-event-checker plugins remove
```

## `custom-event-checker plugins:uninstall PLUGIN...`

Removes a plugin from the CLI.

```
USAGE
  $ custom-event-checker plugins:uninstall PLUGIN...

ARGUMENTS
  PLUGIN  plugin to uninstall

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Removes a plugin from the CLI.

ALIASES
  $ custom-event-checker plugins unlink
  $ custom-event-checker plugins remove
```

## `custom-event-checker plugins:uninstall PLUGIN...`

Removes a plugin from the CLI.

```
USAGE
  $ custom-event-checker plugins:uninstall PLUGIN...

ARGUMENTS
  PLUGIN  plugin to uninstall

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Removes a plugin from the CLI.

ALIASES
  $ custom-event-checker plugins unlink
  $ custom-event-checker plugins remove
```

## `custom-event-checker plugins update`

Update installed plugins.

```
USAGE
  $ custom-event-checker plugins update [-h] [-v]

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Update installed plugins.
```

## `custom-event-checker validateEvents`

Build a file with the unknown properties per event

```
USAGE
  $ custom-event-checker validateEvents -f <value> -o <value>

FLAGS
  -f, --configFile=<value>  (required) [default: ./defaultConfig.json] JSON configuration file location
  -o, --out=<value>         (required) [default: ./data/error.json] Exported file name

DESCRIPTION
  Build a file with the unknown properties per event

EXAMPLES
  $ oex validateEvents --configFile=./path/to/your/config/config.json
    Start the events analysis
    Looking for configuration in file ./defaultConfig.json
    Processed 315 events in 1546 ms
```

_See code: [dist/commands/validateEvents/index.ts](https://github.com/jsinovassin/custom-event-checker/blob/v0.1.0/dist/commands/validateEvents/index.ts)_
<!-- commandsstop -->
