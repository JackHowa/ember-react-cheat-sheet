# Fragment

## Ember 

In Ember.js, you can return multiple elements naturally because Ember templates allow this without the explicit need for a wrapper component.

```hbs
Text outside
<p data-test-text-inside>Text inside</p>
```

## React 

React components can only return one root node. A Fragment is a lightweight wrapper that lets you group multiple elements without adding extra nodes to the DOM. This is particularly useful when a component needs to return multiple sibling elements.


```jsx
const TextContainer = () => (
  <>
    Text outside
    <p data-test-text-inside>Text inside</p>
  </>
);

export default TextContainer;
```