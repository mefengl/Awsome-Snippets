# Awsome-Snippets

People should have their own snippet.

## HTML
https://github.com/abusaidm/html-snippets

## JavaScript

https://github.com/xabikos/vscode-javascript ⭐️

https://github.com/DonJayamanne/jquerysnippets

https://github.com/johnpapa/vscode-angular-snippets

https://github.com/burkeholland/simple-react-snippets

https://github.com/chillios-ts/vscode-react-javascript-snippets

https://github.com/hollowtree/vscode-vue-snippets

## My Own

```js
{
  // cmmb
  "commentBigBlock": {
    "prefix": "cmmb",
    "body": ["/**", " * ${1:first}", " */"],
    "scope": "typescript,typescriptreact,javascript,javascriptreact"
  },

  // cgr cge clg clo cls
  "consoleClear": {
    "prefix": "cls",
    "body": ["console.clear();", "$0"],
    "description": "Clears the console"
  },
  "consoleGroup": {
    "prefix": "cgr",
    "body": ["console.group('log group');", "$0", "console.groupEnd();"],
    "description": "Groups and indents all following output by an additional level, until console.groupEnd() is called."
  },
  "consoleLog": {
    "prefix": "clg",
    "body": ["console.log(${1:object});", "$0"],
    "description": "Displays a message in the console"
  },
  "consoleLogObject": {
    "prefix": "clo",
    "body": ["console.log('${1:object} :>> ', ${1:object});", "$0"],
    "description": "Displays an object in the console with its name"
  },

  // imp imn imd
  "import": {
    "prefix": "imp",
    "body": "import ${2:moduleName} from '${1:module}';$0",
    "description": "Imports entire module statement in ES6 syntax"
  },
  "importNoModuleName": {
    "prefix": "imn",
    "body": "import '${1:module}';$0",
    "description": "Imports entire module in ES6 syntax without module name"
  },
  "importDestructing": {
    "prefix": "imd",
    "body": "import { $2 } from '${1:module}';$0",
    "description": "Imports only a portion of the module in ES6 syntax"
  },
  "exportEverything": {
    "prefix": "ex-router",
    "body": [
      "export * from '${1:module}';",
      "export { default } from '${1:module}';$0"
    ],
    "description": "Exports everything from a module, so that the module doesn't need to be named 'index.tsx'"
  },

  // edf
  "exportDefaultFunction": {
    "prefix": "edf",
    "body": "export default function ${1:${TM_FILENAME_BASE}}(${2:params}) {\n\t$0\n};\n",
    "description": "Export default function in ES6 syntax"
  },

  // fre
  "forEach": {
    "prefix": "fre",
    "body": "${1:array}.forEach(${2:currentItem} => {\n\t${0}\n});",
    "description": "Creates a forEach statement in ES6 syntax"
  },

  // nfn anfn
  "namedFunction": {
    "prefix": "nfn",
    "body": "const ${1:name} = (${2:params}) => {\n\t${3}\n}",
    "description": "Creates a named function in ES6 syntax"
  },
  "anonymousFunction": {
    "prefix": "anfn",
    "body": "(${1:params}) => {\n\t${2}\n}",
    "description": "Creates an anonymous function in ES6 syntax"
  },

  // dob dar
  "destructingObject": {
    "prefix": "dob",
    "body": "const {${2:propertyName}} = ${1:objectToDestruct};",
    "description": "Creates and assigns a local variable using object destructing"
  },
  "destructingArray": {
    "prefix": "dar",
    "body": "const [${2:propertyName}] = ${1:arrayToDestruct};",
    "description": "Creates and assigns a local variable using array destructing"
  },

  /**
   * React
   */
  // fc
  "Function Syntax Component": {
    "prefix": "fc",
    "body": [
      "export default function $1($2) {",
      "$0",
      "\treturn ( <>I am $1</> );",
      "}"
    ],
    "description": "Function Syntax Component"
  },

  // uef ust
  "useEffect": {
    "prefix": "uef",
    "body": ["useEffect(() => {", "\t$1", "}, []);"],
    "description": "useEffect Hook"
  },
  "Declare a new state variable using State Hook": {
    "prefix": "ust",
    "body": ["const [${1}, set${1/(.*)/${1:/capitalize}/}] = useState($2);"],
    "description": "Declare a new state Variable using the State Hook. Hit Tab to apply CamelCase to function"
  }
}
```
