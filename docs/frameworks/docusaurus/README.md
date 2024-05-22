<!-- Basic Github README.MD Header -->
<div style="text-align: right;"> 
	<a href="https://annebrown.ca">
		<img src="../../static/img/logo-ab.png" width="20"/>
	</a> 
	annebrown.ca
</div>
<div style="text-align: right;">
	<sub>
		<a href="https://github.com/annebrown/?tab=repositories">MyRepos</a>
		/docs-priv/frameworks/docusaurus/README.md
	</sub>
 </div>
<!-- End of Header -->

# Docusaurus

## Create New Docusaurus Site

```bash
anne@host:~ $ npx create-docusaurus@latest new-doc-dir classic --typescript
```

All npm/npx commands are executed from within the project folder.

```bash
$ cd /path-to/new-doc-dir
```

Start server at [http://localhost:3000](http://localhost:3000)

```bash
$ cd new-doc-dir
$ npm run start
```

The server builds if rqd.

## Deploy

Build static files for production in the `new-doc-dir/build` directory:

```bash
npm run build
```

Stage/Test/Review locally:

```bash
npm run serve
```

Review changes at: [http://localhost:3000](http://localhost:3000)

Configure docusaurus.config.ts

Backing out of Blunders

Close VSCode.

Delete local project directory.

Clone using docusaurus:

```bash
npx create-docusaurus@latest https://annebrown@github.com/annebrown/docs.git
npm run build
```

Check deployment host.


## Docusaurus Mods

### Remove blog

Delete the directory.

```bash
$ rm -rf blog
```

Add to Docosaurus Config:

```json
blog:false
```

## CFL

### Docusaurus Config

Edit these lines in `docusaurus.config.ts`:

```json
title: 'Documentation',
tagline: 'Docs for browndomain.com',
favicon: 'img/favicon.ico',
url: 'https://docs.browndomain.com',
baseUrl: '/',
```

Delete this line to remove "Edit this Page" links.

```json
editUrl: 'https://github.com/facebook/docusaurus/tree/main/packages/create-docusaurus/templates/shared/',
```

Remove `blog: { ... }` from presets.

Edit remaining stuff in doco cofig to suit rqd theming, content structure, copyright, social media links, etc.

Files

```
/README.md
/src/pages/index.tsx
```

## Backing out of Blunders

Close VSCode.

Delete local project directory.

Clone using docusaurus:

```bash
npx create-docusaurus@latest https://annebrown@github.com/annebrown/docs.git
npm run build
```

Check deployment host.

