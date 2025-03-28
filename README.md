# events

Small event emitter

```ts
const emitter = new EventEmitter<{
	add: [text: string];
	clear: [];
}>();

emitter.on('add', (text) => {
	console.log({ text });
});

emitter.emit('add', `Hello world!`);
```
