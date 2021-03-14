# Today I Learned

## JSX Interpolation
In order to use JavaScript Expression one has to use `{}`, the curly brackets. So let's say there is a JavaScript element like below.
```jsx
let data = {
  contents: 'This is a test',
}
```
and to use `Interpolation` you can use it like below.
```jsx
const testElement = <h1>{data.content}</h1>
```
With interpolation you can also add attributes. Like title, style, class, id, for..
The thing that you have to be careful is that because even if this might still look like an HTML syntax it's actually JSX. So `class` would be `className`. Always use it in `camelCase`!!. However with accessibility you can still use `aria-label` and `role` as it is. 
Also make sure to use only one root element!!! So you cannot use it like below.
```jsx
const ButtonGroup = (
  <button type="button" className="button button__save">Save</button>
  <button type="button" className="button button__cancel">Cancel</button>
)
```
instead you have to write it like this. 
```jsx
const ButtonGroup = (
  <div className="button-group">
    <button type="button" className="button button__save">Save</button>
    <button type="button" className="button button__cancel">Cancel</button>
  </div>
)
```
but also with the above if you don't have any intention of wrapping it you can use `React.Fragment` using `import React from 'react'` on the top of the js file. Or even `<></>`.
  