# Events
There are some events you can listen for. A full list of events can be found [here](/api/classes.md#editor-options).

```js
const editor = new Editor({
  onInit: () => {
    // editor is initialized
  },
  onUpdate: ({ getHTML }) => {
    // get new content on update
    const newContent = this.getHTML()
  },
})
```

It's also possible to register event listeners afterwards.

```js
const editor = new Editor()

editor.on('init', () => {
  // editor is initialized
})

editor.on('update', ({ getHTML }) => {
  // get new content on update
  const newContent = this.getHTML()
})
```