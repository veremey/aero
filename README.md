In this case HTML5 only. No JS.   🦴

## Installation

```bash
npm i -g npm
```
```shell
npm install -g gulp
```

[Download TARS](../../../tars/archive/master.zip) and unzip it in the working directory. Then install dependencies. Command is run from a folder with TARS files (usually it is a tars-master).

```shell
npm install
```

In tars-master remove  ` markup `. Put here path from Aero project

```shell
gulp init
```

Start whith
`gulp dev --lr`

Enjoy yourself!


## Basic commands

**Attention, [TARS-CLI](https://github.com/tars/tars-cli) is the preferred
 way to work with TARS. It is faster and more comfortable to work with TARS-CLI. All commands are available and [described in TARS-CLI](https://github.com/tars/tars-cli/blob/master/docs/en/commands.md), so use only TARS-CLI for working with your project. TARS used Gulp to start tasks, when CLI was not created.**

`gulp init` — initializes project with the specified settings in the tars-config. Creates a file structure.

`gulp re-init` — **This command is deprecated!** reinitialize the project with specified settings in the tars-config. It is advised to use this command if you initialize the project with incorrect options. **Attention, files from pages and static folder will be deleted.**

`gulp` or `gulp build` — build project. Non-minimized files are used by default. Build type depends on command parameters.
Available parameters:

* `--min` – minimized files are connected to html.
* `--release` – minimized  files are connected to html whose names have hash. This mode is useful if you are trying to directly deploy ready markup to the server.

`gulp dev` — initialize of builder in development mode. Dev-version of the project is created  without any minifications. It also launches watchers for project files.
Available parameters:

* `--lr` – initialize livereload (live page reloads with changes in project files), if it is included in the configuration of the project.
* `--tunnel` – initialize project with markup sharing to the external web.

The link will be shown in the console. There also will be a link to the control panel for devices to which markup is shared.

`gulp build-dev` — generation of dev-version of the project without watchers.

These parameters are available in any mode of assembly:

* `--ie8` – to include in the build styles for ie8.
* `--ie9` – to include in the build styles for ie9.
* `--ie` – to include in the build styles for ie8 and ie9.


## Documentation

It is important! All examples in documentation use the default settings.

* [File structure](/docs/en/file-structure.md)
* [Working with tasks and watchers](/docs/en/tasks-and-watchers.md)
* [TARS Options](/docs/en/options.md)
* [Plugins configuration](/docs/en/plugins-options.md)
* [Html](/docs/en/html-processing.md)
* [Css](/docs/en/css-processing.md)
* [Js](/docs/en/js-processing.md)
* [Working with images](/docs/en/images-processing.md)
* [Working with fonts and misc-files](/docs/en/fonts-and-misc.md)
* [Usage script (scenarios)](/docs/en/scenarios.md)
* [Upgrade guide](/docs/en/update-guide.md)
* [FAQ](/docs/en/faq.md)

