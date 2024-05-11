# @hoangcung1804npm/excepturi-facilis-rerum

[![npm](https://img.shields.io/npm/v/@hoangcung1804npm/excepturi-facilis-rerum)](https://www.npmjs.com/package/@hoangcung1804npm/excepturi-facilis-rerum)

`@hoangcung1804npm/excepturi-facilis-rerum` is a node command line tool to generate directory structure tree.

## Installation

```bash
npm i @hoangcung1804npm/excepturi-facilis-rerum -g
```

## Usage

```bash
$ @hoangcung1804npm/excepturi-facilis-rerum -h
Usage: @hoangcung1804npm/excepturi-facilis-rerum [options]

Generate a directory structure tree

Options:
  -V, --version          output the version number
  -i, --ignore <ig>      ignore specific directory name, separated by comma or '|'  
  -l, --layer <layer>    specify the layer of output
  -d, --directory <dir>  specify the directory to generate structure tree
  -f, --only-folder      output folder only
  --icon                 output emoji icon, prefixing filename or directory
  -o, --output <output>  export content into a file, appending mode by default      
  -h, --help             display help for command
```

## Examples

Ignore `.git` and `node_modules` directory.

```bash
$ @hoangcung1804npm/excepturi-facilis-rerum -i '.git|node_modules' # or @hoangcung1804npm/excepturi-facilis-rerum -i '.git,node_modules'
@hoangcung1804npm/excepturi-facilis-rerum
├──📄.editorconfig
├──📄.eslintrc.js
├──📄.gitignore
├──📄.prettierrc.js
├──📄.release-it.json
├──📄CHANGELOG.md
├──📄LICENSE
├──📄package-lock.json
├──📄package.json
├──📄README.md
└──📁src
    ├──📄config.js
    ├──📄generate.js
    ├──📄index.js
    ├──📄toTree.js
    └──📄utils.js
```

Show emoji icon, prefixing filename or directory.

```bash
$ @hoangcung1804npm/excepturi-facilis-rerum -i '.git,node_modules' --icon
@hoangcung1804npm/excepturi-facilis-rerum
├──📄.editorconfig
├──📄.eslintrc.js
├──📄.gitignore
├──📄.prettierrc.js
├──📄.release-it.json
├──📄CHANGELOG.md
├──📄LICENSE
├──📄package-lock.json
├──📄package.json
├──📄README.md
└──📁src
    ├──📄config.js
    ├──📄generate.js
    ├──📄index.js
    ├──📄toTree.js
    └──📄utils.js
```

Export output into `result.md`, and append mode by default.

```bash
$ @hoangcung1804npm/excepturi-facilis-rerum -i '.git,node_modules' -o result.md
@hoangcung1804npm/excepturi-facilis-rerum
├──📄.editorconfig
├──📄.eslintrc.js
├──📄.gitignore
├──📄.prettierrc.js
├──📄.release-it.json
├──📄CHANGELOG.md
├──📄LICENSE
├──📄package-lock.json
├──📄package.json
├──📄README.md
└──📁src
    ├──📄config.js
    ├──📄generate.js
    ├──📄index.js
    ├──📄toTree.js
    └──📄utils.js
```
## License

[MIT](./LICENSE)
