# REACT.js

## Conditional Rendering

- Conditional rendering in React works the same way conditions work in JavaScript. Use JavaScript operators like if or the conditional operator to create elements representing the current state, and let React update the UI to match them.

- Element Variables You can use variables to store elements. This can help you conditionally render a part of the component while the rest of the output doesn’t change.
    Inline If with Logical && Operator

- You may embed expressions in JSX by wrapping them in curly braces. This includes the JavaScript logical && operator. It can be handy for conditionally including an element: 
``` 
function Mailbox(props) { const unreadMessages = props.unreadMessages; return (
Hello!
{unreadMessages.length > 0 &&
You have {unreadMessages.length} unread messages.
}
); }

const messages = [‘React’, ‘Re: React’, ‘Re:Re: React’]; ReactDOM.render( <Mailbox unreadMessages={messages} />, document.getElementById(‘root’) );
```

## Lists and Keys
1. Lists :
- Given the code below, we use the map() function to take an array of numbers and double their values. We assign the new array returned by map() to the variable doubled and log it:

```
const numbers = [1, 2, 3, 4, 5];
const doubled = numbers.map((number) => number * 2);
console.log(doubled);

```
> This code logs [2, 4, 6, 8, 10] to the console.

- In React, transforming arrays into lists of elements is nearly identical.

- Rendering Multiple Components
- You can build collections of elements and include them in JSX using curly braces {}.

- Below, we loop through the numbers array using the JavaScript map() function. We return a <li> element for each item. Finally, we assign the resulting array of elements to listItems:
```
const numbers = [1, 2, 3, 4, 5];
const listItems = numbers.map((number) =>
<li>{number}</li>
);

```
We include the entire listItems array inside a <ul> element, and render it to the DOM:

```
ReactDOM.render(
<ul>{listItems}</ul>,
document.getElementById('root')
);

```

2. Keys

- Keys help React identify which items have changed, are added, or are removed.

### Extracting Components with Keys
- Keys only make sense in the context of the surrounding array.

- For example, if you extract a ListItem component, you should keep the key on the <ListItem /> elements in the array rather than on the <li> element in the ListItem itself.



