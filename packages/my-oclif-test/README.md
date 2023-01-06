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
$ npm install -g my-oclif-test
$ my-oclif-test COMMAND
running command...
$ my-oclif-test (--version)
my-oclif-test/0.0.0 darwin-x64 node-v16.19.0
$ my-oclif-test --help [COMMAND]
USAGE
  $ my-oclif-test COMMAND
...
```
<!-- usagestop -->
# Commands
<!-- commands -->
* [`my-oclif-test hello PERSON`](#my-oclif-test-hello-person)
* [`my-oclif-test hello world`](#my-oclif-test-hello-world)
* [`my-oclif-test help [COMMAND]`](#my-oclif-test-help-command)
* [`my-oclif-test plugins`](#my-oclif-test-plugins)
* [`my-oclif-test plugins:install PLUGIN...`](#my-oclif-test-pluginsinstall-plugin)
* [`my-oclif-test plugins:inspect PLUGIN...`](#my-oclif-test-pluginsinspect-plugin)
* [`my-oclif-test plugins:install PLUGIN...`](#my-oclif-test-pluginsinstall-plugin-1)
* [`my-oclif-test plugins:link PLUGIN`](#my-oclif-test-pluginslink-plugin)
* [`my-oclif-test plugins:uninstall PLUGIN...`](#my-oclif-test-pluginsuninstall-plugin)
* [`my-oclif-test plugins:uninstall PLUGIN...`](#my-oclif-test-pluginsuninstall-plugin-1)
* [`my-oclif-test plugins:uninstall PLUGIN...`](#my-oclif-test-pluginsuninstall-plugin-2)
* [`my-oclif-test plugins update`](#my-oclif-test-plugins-update)

## `my-oclif-test hello PERSON`

Say hello

```
USAGE
  $ my-oclif-test hello [PERSON] -f <value>

ARGUMENTS
  PERSON  Person to say hello to

FLAGS
  -f, --from=<value>  (required) Who is saying hello

DESCRIPTION
  Say hello

EXAMPLES
  $ oex hello friend --from oclif
  hello friend from oclif! (./src/commands/hello/index.ts)
```

_See code: [dist/commands/hello/index.ts](https://github.com/v-mosuna/hello-world/blob/v0.0.0/dist/commands/hello/index.ts)_

## `my-oclif-test hello world`

Say hello world

```
USAGE
  $ my-oclif-test hello world

DESCRIPTION
  Say hello world

EXAMPLES
  $ my-oclif-test hello world
  hello world! (./src/commands/hello/world.ts)
```

## `my-oclif-test help [COMMAND]`

Display help for my-oclif-test.

```
USAGE
  $ my-oclif-test help [COMMAND] [-n]

ARGUMENTS
  COMMAND  Command to show help for.

FLAGS
  -n, --nested-commands  Include all nested commands in the output.

DESCRIPTION
  Display help for my-oclif-test.
```

_See code: [@oclif/plugin-help](https://github.com/oclif/plugin-help/blob/v5.1.22/src/commands/help.ts)_

## `my-oclif-test plugins`

List installed plugins.

```
USAGE
  $ my-oclif-test plugins [--core]

FLAGS
  --core  Show core plugins.

DESCRIPTION
  List installed plugins.

EXAMPLES
  $ my-oclif-test plugins
```

_See code: [@oclif/plugin-plugins](https://github.com/oclif/plugin-plugins/blob/v2.1.12/src/commands/plugins/index.ts)_

## `my-oclif-test plugins:install PLUGIN...`

Installs a plugin into the CLI.

```
USAGE
  $ my-oclif-test plugins:install PLUGIN...

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
  $ my-oclif-test plugins add

EXAMPLES
  $ my-oclif-test plugins:install myplugin 

  $ my-oclif-test plugins:install https://github.com/someuser/someplugin

  $ my-oclif-test plugins:install someuser/someplugin
```

## `my-oclif-test plugins:inspect PLUGIN...`

Displays installation properties of a plugin.

```
USAGE
  $ my-oclif-test plugins:inspect PLUGIN...

ARGUMENTS
  PLUGIN  [default: .] Plugin to inspect.

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Displays installation properties of a plugin.

EXAMPLES
  $ my-oclif-test plugins:inspect myplugin
```

## `my-oclif-test plugins:install PLUGIN...`

Installs a plugin into the CLI.

```
USAGE
  $ my-oclif-test plugins:install PLUGIN...

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
  $ my-oclif-test plugins add

EXAMPLES
  $ my-oclif-test plugins:install myplugin 

  $ my-oclif-test plugins:install https://github.com/someuser/someplugin

  $ my-oclif-test plugins:install someuser/someplugin
```

## `my-oclif-test plugins:link PLUGIN`

Links a plugin into the CLI for development.

```
USAGE
  $ my-oclif-test plugins:link PLUGIN

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
  $ my-oclif-test plugins:link myplugin
```

## `my-oclif-test plugins:uninstall PLUGIN...`

Removes a plugin from the CLI.

```
USAGE
  $ my-oclif-test plugins:uninstall PLUGIN...

ARGUMENTS
  PLUGIN  plugin to uninstall

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Removes a plugin from the CLI.

ALIASES
  $ my-oclif-test plugins unlink
  $ my-oclif-test plugins remove
```

## `my-oclif-test plugins:uninstall PLUGIN...`

Removes a plugin from the CLI.

```
USAGE
  $ my-oclif-test plugins:uninstall PLUGIN...

ARGUMENTS
  PLUGIN  plugin to uninstall

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Removes a plugin from the CLI.

ALIASES
  $ my-oclif-test plugins unlink
  $ my-oclif-test plugins remove
```

## `my-oclif-test plugins:uninstall PLUGIN...`

Removes a plugin from the CLI.

```
USAGE
  $ my-oclif-test plugins:uninstall PLUGIN...

ARGUMENTS
  PLUGIN  plugin to uninstall

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Removes a plugin from the CLI.

ALIASES
  $ my-oclif-test plugins unlink
  $ my-oclif-test plugins remove
```

## `my-oclif-test plugins update`

Update installed plugins.

```
USAGE
  $ my-oclif-test plugins update [-h] [-v]

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Update installed plugins.
```
<!-- commandsstop -->
