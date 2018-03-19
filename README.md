# slate-editor-icons [![NPM version][npm-image]][npm-url] [![Build Status][travis-image]][travis-url] [![Dependency Status][daviddm-image]][daviddm-url]
> Shared icon and render functions for slate editors, icons is extracted from [Quill editor](https://quilljs.com/) (see [quill-icons](https://github.com/Canner/quill-icons) for more information)

## Usage

This project is maintain in a monorepo, see packages in `packages` folder

## Icon packages

### @canner/slate-icon-align

Export components:

- AlignCenter
- AlignLeft
- AlignRight

```js
import {AlignCenter, AlignLeft, AlignRight} from '@canner/slate-icon-align';
```

### @canner/slate-icon-blockquote

```js
import Blockquote from 'packages/slate-icon-blockquote';
```

### @canner/slate-icon-bold

### @canner/slate-icon-clean

### @canner/slate-icon-code

### @canner/slate-icon-emoji

### @canner/slate-icon-fontBgColor

### @canner/slate-icon-fontColor

### @canner/slate-icon-header

Export components: 
  - Header1
  - Header2

### @canner/slate-icon-image

### @canner/slate-icon-indent

Export components:
  - Indent
  - Outdent

### @canner/slate-icon-italic

### @canner/slate-icon-link

### @canner/slate-icon-list

### @canner/slate-icon-strikethrough

### @canner/slate-icon-underline

### @canner/slate-icon-undo

### @canner/slate-icon-video

### @canner/slate-icon-rendernodes

## Usage

Install icons you want to support in your project, and pass slate editor `Change` and `onChange` function into the component. When users click these icons it will apply changes the called onChange function to update new change to slate editor.

You will need to pass customized icon classname props to your components ([supported classes](https://github.com/Canner/quill-icons#props)), you could look at the example [to setup your icon's styles](https://github.com/Canner/slate-editor-icons/blob/master/docs/style.css) 


The best explanation is a simple example: https://github.com/Canner/slate-editor-icons/blob/master/docs/index.js

## Icon Props

| **props** | **type** | **required** | **default** | **description**  |
|-----------|----------|--------------|-------------|------------------|
| change     | object   | true        | null          | changes to value |
| onChange  | func   | true         | null         | onChange function usually `change => this.setState({value})` to update slate state  |


## Start example server

```
node start
```

## Maintainer

[chilijung](https://github.com/chilijung)

## License

MIT © [Canner](https://github.com/Canner)


[npm-image]: https://badge.fury.io/js/slate-editor-icons.svg
[npm-url]: https://npmjs.org/package/slate-editor-icons
[travis-image]: https://travis-ci.org/Canner/slate-editor-icons.svg?branch=master
[travis-url]: https://travis-ci.org/Canner/slate-editor-icons
[daviddm-image]: https://david-dm.org/Canner/slate-editor-icons.svg?theme=shields.io
[daviddm-url]: https://david-dm.org/Canner/slate-editor-icons
