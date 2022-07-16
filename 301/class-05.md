### Putting it all together

## Reading

[React Docs - Thinking in React](https://reactjs.org/docs/thinking-in-react.html)

- What is the single responsibility principle and how does it apply to components?
    - single responsibility indicates that a component or function should just do one thing.  If it does more, make seperate components
- What does it mean to build a ‘static’ version of your application?
    - non interactive
- Once you have a static application, what do you need to add?
    - interaction
- What are the three questions you can ask to determine if something is state?
    - is it passed in or handled within the component?
    - does it change over time?
    - Can you compute it based on any other state or props in your component?
- How can you identify where state needs to live?
    - identify every component that renders something based on that state.
    - find a common owner component
    - either the common owner or another component higher up should own the state
    - if you can't find a component where it makes sense to own the state, create a new component solely for holding the state and add it somewhere in the hierarchy above the common owner component

[Higher-Order Functions](https://eloquentjavascript.net/05_higher_order.html#h_xxCc98lOBK)

- What is a “higher-order function”?
    - functions that operate on other functions, either by taking them as arguments or by returning them
- Explore the greaterThan function as defined in the reading. 
```js
function greaterThan(n) {
  return m => m > n;
}
let greaterThan10 = greaterThan(10);
console.log(greaterThan10(11));
// → true
```
- In your own words, what is line 2 of this function doing?
    - returning the first number that is greater than the argument?
- Explain how either map or reduce operates, with regards to higher-order functions.
    - map and reduce both iterate over the items in an array and perform another function on each.  They are both higher order functions.

## Things I want to know more about

- Higher-order functions allow us to abstract over <i style="color:#E88C17; font-size: 110%" >actions</i>, not just values.
    - what does this mean, what is abstracting over actions, not just values?
- Why aren't our labs presented more in line with how the first reading shows us how we should be thinking for react products.  We don't conceptualize, then start with a mock, then break the ui into a component hierarchy, followed by building a static version etc.