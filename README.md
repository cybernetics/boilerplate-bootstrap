# boilerplate-bootstrap [![NPM version](https://badge.fury.io/js/boilerplate-bootstrap.png)](http://badge.fury.io/js/boilerplate-bootstrap)

> Build Bootstrap with Assemble instead of Jekyll.

#### [See it live →](http://assemble.github.io/boilerplate-bootstrap/)

* Converts the liquid templates to Handlebars
* Builds the HTML from templates using [Assemble][assemble].
* Swaps out some Bootstrap content with metadata from [_config.yml](./_config.yml).

## Quickstart
_You must have [NPM](npmjs.org), [Bower][bower] and [Grunt][grunt] installed globally before you begin._

#### 1. Download this project
Do _one_ of the following:

* **[download][download]** this project
* `git clone git://github.com/assemble/boilerplate-bootstrap.git`
* `bower install boilerplate-bootstrap`

#### 2. Next, install Bootstrap and dependencies
Next, `cd` into the project run the following in the command line:

```bash
npm i && git clone git://github.com/twbs/bootstrap.git "vendor/bootstrap" && cd vendor/bootstrap && npm i
```

#### 3. Customize [_config.yml](./_config.yml)
Optionally update the metadata and config defaults to how you want them for your project.


#### 4. Last, build.
You may now run `grunt` to build the project.


## The "assemble" task
If you haven't used [Assemble][assemble] before, please visit [http://assemble.io/docs](http://assemble.io/docs) to learn how to customize the task.

### Overview
In the project's Gruntfile, the example `assemble` task is pre-loaded with paths and options to build the project successfully:

```js
assemble: {
  options: {
    flatten: true,
    assets: '<%= site.assets %>',

    // Metadata
    site: '<%= site %>',

    // Templates
    partials: '<%= site.includes %>',
    layoutdir: '<%= site.layouts %>',
    layout: '<%= site.layout %>',
  },
  docs: {
    src: ['templates/*.hbs'],
    dest: '<%= site.dest %>/'
  }
}
```

Take a look at [_config.yml](./_config.yml) to see some of the metadata and config data is defined.



## Author

**Jon Schlinkert**

+ [http://github.com/jonschlinkert](http://github.com/jonschlinkert)
+ [http://twitter.com/jonschlinkert](http://twitter.com/jonschlinkert)


## Contributing
In lieu of a formal styleguide, take care to maintain the existing coding style. Add unit tests for any new or changed functionality.


## Release History
* 2013-12-22    v0.2.6    Updated dependencies, Bootstrap paths. A number of updates to gruntfile and config. Adds _config.yml to project root, to make project metadata more customizable from the start.
* 2013-08-03    v0.2.0    Refactored to be awesome.
* 2013-07-16    v0.1.0    First commit.


[download]: https://github.com/assemble/boilerplate-bootstrap/archive/master.zip "Download boilerplate-bootstrap"
[helpers]: https://github.com/assemble/handlebars-helpers "Handlebars Helpers"
[assemble]: https://github.com/assemble/assemble/ "Assemble"
[assemble-boilerplates]: https://github.com/assemble/assemble-boilerplates "Assemble Boilerplates"

[bower]: https://github.com/bower/bower
[grunt]: http://gruntjs.com
[gruntfile]: http://gruntjs.com/sample-gruntfile
[configuring tasks]: http://gruntjs.com/configuring-tasks
[tasks-and-targets]: http://gruntjs.com/configuring-tasks#task-configuration-and-targets
[files-object]: http://gruntjs.com/configuring-tasks#building-the-files-object-dynamically