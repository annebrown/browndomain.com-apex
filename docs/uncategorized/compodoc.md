### Stuff for Docs



Need more than Markdown



Easier nav between docs



# compodoc



# Description



# Usage



### Assumptions

Angjular webapp exists, along with all deps, including

- Node.js

- Angular-CLI



### Install

```bash
cd angular-app
npm install -g @compodoc/compodoc
 
```

### Config

```tsconfig.doc.json```:

```js
{
    "include": ["src/**/*.ts"]'
    "exclude": ["src/tes.ts", "src/**.*.spec.ts", "src/app/fil-to-exclude.ts"]
}
```

Add script task to ```package.json```:

```js 
"scripts": {
    "compodoc": "npm compodoc -p tsconfig.doc.json"
}
```

### Run

```bash
npm run compodoc
```

```

## Config Files

```bash
angular-app-root/.compodocrc
```

or

```bash
angular-app-root/.compodocrc.json
```

or, a compodoc property in ```package.json```.










