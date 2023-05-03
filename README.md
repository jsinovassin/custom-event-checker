oclif-hello-world
=================

oclif example Hello World CLI

[![oclif](https://img.shields.io/badge/cli-oclif-brightgreen.svg)](https://oclif.io)
[![Version](https://img.shields.io/npm/v/oclif-hello-world.svg)](https://npmjs.org/package/oclif-hello-world)
[![CircleCI](https://circleci.com/gh/oclif/hello-world/tree/main.svg?style=shield)](https://circleci.com/gh/oclif/hello-world/tree/main)
[![Downloads/week](https://img.shields.io/npm/dw/oclif-hello-world.svg)](https://npmjs.org/package/oclif-hello-world)
[![License](https://img.shields.io/npm/l/oclif-hello-world.svg)](https://github.com/oclif/hello-world/blob/main/package.json)

<!-- toc -->
* [Usage](#usage)
* [Commands](#commands)
<!-- tocstop -->
# Usage
<!-- usage -->
```sh-session
$ npm install -g custom-event-checker
$ custom-event-identifier COMMAND
running command...
$ custom-event-identifier (--version)
custom-event-identifier/0.0.0 darwin-x64 node-v19.4.0
$ custom-event-identifier --help [COMMAND]
USAGE
  $ custom-event-identifier COMMAND
...
```
<!-- usagestop -->
# Commands
<!-- commands -->
* [`custom-event-identifier help [COMMANDS]`](#custom-event-identifier-help-commands)
* [`custom-event-identifier plugins`](#custom-event-identifier-plugins)
* [`custom-event-identifier plugins:install PLUGIN...`](#custom-event-identifier-pluginsinstall-plugin)
* [`custom-event-identifier plugins:inspect PLUGIN...`](#custom-event-identifier-pluginsinspect-plugin)
* [`custom-event-identifier plugins:install PLUGIN...`](#custom-event-identifier-pluginsinstall-plugin-1)
* [`custom-event-identifier plugins:link PLUGIN`](#custom-event-identifier-pluginslink-plugin)
* [`custom-event-identifier plugins:uninstall PLUGIN...`](#custom-event-identifier-pluginsuninstall-plugin)
* [`custom-event-identifier plugins:uninstall PLUGIN...`](#custom-event-identifier-pluginsuninstall-plugin-1)
* [`custom-event-identifier plugins:uninstall PLUGIN...`](#custom-event-identifier-pluginsuninstall-plugin-2)
* [`custom-event-identifier plugins update`](#custom-event-identifier-plugins-update)
* [`custom-event-identifier validateEvents PERSON`](#custom-event-identifier-validateevents-person)

## `custom-event-identifier help [COMMANDS]`

Display help for custom-event-identifier.

```
USAGE
  $ custom-event-identifier help [COMMANDS] [-n]

ARGUMENTS
  COMMANDS  Command to show help for.

FLAGS
  -n, --nested-commands  Include all nested commands in the output.

DESCRIPTION
  Display help for custom-event-identifier.
```

_See code: [@oclif/plugin-help](https://github.com/oclif/plugin-help/blob/v5.2.9/src/commands/help.ts)_

## `custom-event-identifier plugins`

List installed plugins.

```
USAGE
  $ custom-event-identifier plugins [--core]

FLAGS
  --core  Show core plugins.

DESCRIPTION
  List installed plugins.

EXAMPLES
  $ custom-event-identifier plugins
```

_See code: [@oclif/plugin-plugins](https://github.com/oclif/plugin-plugins/blob/v2.4.7/src/commands/plugins/index.ts)_

## `custom-event-identifier plugins:install PLUGIN...`

Installs a plugin into the CLI.

```
USAGE
  $ custom-event-identifier plugins:install PLUGIN...

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
  $ custom-event-identifier plugins add

EXAMPLES
  $ custom-event-identifier plugins:install myplugin 

  $ custom-event-identifier plugins:install https://github.com/someuser/someplugin

  $ custom-event-identifier plugins:install someuser/someplugin
```

## `custom-event-identifier plugins:inspect PLUGIN...`

Displays installation properties of a plugin.

```
USAGE
  $ custom-event-identifier plugins:inspect PLUGIN...

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
  $ custom-event-identifier plugins:inspect myplugin
```

## `custom-event-identifier plugins:install PLUGIN...`

Installs a plugin into the CLI.

```
USAGE
  $ custom-event-identifier plugins:install PLUGIN...

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
  $ custom-event-identifier plugins add

EXAMPLES
  $ custom-event-identifier plugins:install myplugin 

  $ custom-event-identifier plugins:install https://github.com/someuser/someplugin

  $ custom-event-identifier plugins:install someuser/someplugin
```

## `custom-event-identifier plugins:link PLUGIN`

Links a plugin into the CLI for development.

```
USAGE
  $ custom-event-identifier plugins:link PLUGIN

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
  $ custom-event-identifier plugins:link myplugin
```

## `custom-event-identifier plugins:uninstall PLUGIN...`

Removes a plugin from the CLI.

```
USAGE
  $ custom-event-identifier plugins:uninstall PLUGIN...

ARGUMENTS
  PLUGIN  plugin to uninstall

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Removes a plugin from the CLI.

ALIASES
  $ custom-event-identifier plugins unlink
  $ custom-event-identifier plugins remove
```

## `custom-event-identifier plugins:uninstall PLUGIN...`

Removes a plugin from the CLI.

```
USAGE
  $ custom-event-identifier plugins:uninstall PLUGIN...

ARGUMENTS
  PLUGIN  plugin to uninstall

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Removes a plugin from the CLI.

ALIASES
  $ custom-event-identifier plugins unlink
  $ custom-event-identifier plugins remove
```

## `custom-event-identifier plugins:uninstall PLUGIN...`

Removes a plugin from the CLI.

```
USAGE
  $ custom-event-identifier plugins:uninstall PLUGIN...

ARGUMENTS
  PLUGIN  plugin to uninstall

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Removes a plugin from the CLI.

ALIASES
  $ custom-event-identifier plugins unlink
  $ custom-event-identifier plugins remove
```

## `custom-event-identifier plugins update`

Update installed plugins.

```
USAGE
  $ custom-event-identifier plugins update [-h] [-v]

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Update installed plugins.
```

## `custom-event-identifier validateEvents PERSON`

Build a file with the unknown properties per event

```
USAGE
  $ custom-event-identifier validateEvents PERSON -f <value>

ARGUMENTS
  PERSON  Person to say hello to

FLAGS
  -f, --from=<value>  (required) Who is saying hello

DESCRIPTION
  Build a file with the unknown properties per event

EXAMPLES
  $ oex hello friend --from oclif
  hello friend from oclif! (./src/commands/hello/index.ts)
```

_See code: [dist/commands/validateEvents/index.ts](https://github.com/jsinovassin/custom-event-identifier/blob/v0.0.0/dist/commands/validateEvents/index.ts)_
<!-- commandsstop -->
