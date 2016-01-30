# My Little Pony Episode Database

This is a work in progress.

## Development Requirements

|Dependency|OS X Installation|
|:--|:--|
|node.js|`brew install nodejs`|
|gulp|`npm install -g gulp`|
|jspm|`npm install -g jspm`|

## Development

### Installation

```
git clone https://github.com/muffinexplosion/mlp-episode-db.git mlp-episode-db
cd mlp-episode-db
npm install
jspm install
gulp
```

### Live Reload

`gulp`

### Building

`gulp build:<environment>`

After the build the app can be served from __src/app__ directory.

## Environments

* **development**
* **test**
* **staging**
* **production**

## Available Gulp Tasks

|Command|Desc|
|:--|:--|
|`gulp cleanup`|Remove build files|
|`gulp serve` _(default)_|Launch with live reload|
|`gulp set-environment:development`|Set environment to __development__ \*|
|`gulp set-environment:test`|Set environment to __test__ \*|
|`gulp set-environment:staging`|Set environment to __staging__ \*|
|`gulp set-environment:production`|Set environment to __production__ \*|
|`gulp update-revision`|Update current revision based on the git commit or date/time \**|
|`gulp build:development`|Build for the __development__ environment|
|`gulp build:test`|Build for the __test__ environment|
|`gulp build:staging`|Build for the __staging__ environment|
|`gulp build:production`|Build for the __production__ environment|
|`gulp compile-ejs`|Compile EJS files|
|`gulp compile-sass`|Compile SASS files|
|`gulp compile-scripts`|Compile scripts. Creates self-sufficient bundle (except for __development__ environment)|
|`gulp compile-templates`|Compile templates into cache. In __development__ templates are not cached.|
|`gulp optimize-asssets`|Optimize assets|
|`gulp post-build`|Perform post-build steps|

\* Current environment is stored in /environment file

\** Current revision is stored in /revison file


## Author

Muffinexplosion <<muffinexplosion@gmx.net>>.

## License

Basically, [WTFPL](http://www.wtfpl.net/)
