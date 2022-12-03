1. What do props help us accomplish?

- pass in property values to components so we can reuse components across different property values


2. How do you pass a prop into a component?

- just like passing an attribute into an html tag:

```js
<Component prop={value} />
```


3. Can I pass a custom prop (e.g. `blahblahblah={true}`) to a native DOM element? (e.g. <div blahblahblah={true}>) Why or why not?

- no. you can only pass html attributes into native dom elements. you can only pass custom props into custom components

this is valid:
```js
<Component blahblahblah={true}>
```


4. How do I receive props in a component?
```js
function Navbar(props) {
	return (
		<header prop={props.value}>
    ...
    </header>
  )
}
```


5. What data type is `props` when the component receives it?

- an object!