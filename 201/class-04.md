## HTML Links, JS Functions, and Intro to CSS Layout

From the Duckett HTML book:

- Ch4: Ch.4 “**Links**” (pp.74-93)
  - use the &lt;a&gt;
  - **href** attribute indicates the page you are linking to
  - use relative paths when linking within your site
  - can target the id attribute to link to elements in the same page
  - use mailto: to create an email
  - target="_blank" opens link in a new window
  - can link to a specific part of another webpage by using the id at the end of the address
- Ch15: “**Layout**” (pp.358-404)
  - an element's box will be either a block-level or inline box
    - **block-level** - start on a new line
      - examples: &lt;h1&gt;, &lt;p&gt;, &lt;ul&gt;, &lt;li&gt;
    - **inline** - flow in between surrounding text
      - examples: &lt;img&gt;, &lt;b&gt;, &lt;i&gt;
  - **browsers display pages in normal flow unless** you specify relative, absolute, or fixed positioning
        - **normal flow** - each block element gets a new line
        - **relative** - moves the element relative to the position it would have been in normal flow
        - **absolute** - positions an element in relation to its containing element
            - does not affect the position of any surrounding elements
            -
        - **fixed** - form of absolute positioning
            - positions the element in relation to the browser window
                - instead of the containing element
  - floated items require a defined width
  - use z-index if boxes overlap

 Focus your attention on understanding the core concepts presented on pp.358-364, and look at the code samples on the website that accompanies the textbook.

From the Duckett JS book:

- Ch3 (first part): “**Functions, Methods, and Objects**” (pp.86-99 ONLY)
  - **Functions** - serries of statements grouped together to perform a specific task
    - can take parameters and may return a value
    - if different parts of a page require the same task, write a function
    - can return multiple values from a function (p. 95)
      - call the index of the result you want at the end of the function call
      - Example:

```js
function getSize(width, height, depth) {
    let area = width * height;
    let volume = width * height * depth;
    let sizes = [area, volume];
    return sizes 
}

let areaOne = getSize(3, 2, 3)[0];
let volumeOne = getSize(3, 2, 3)[1];
```

- **Object** - series of variables and functions that represent something
  - **properties** - variables in an object
  - **methods** - functions in an object
- JavaScript has built in objects
  - examples: String, Number, Math, and Date
  - their properties and methods offer functionality that help you write js
- global variables take more memory
- [Article](https://www.codefellows.org/blog/6-reasons-for-pair-programming/): “**6 Reasons for Pair Programming**”
  - commonly involves 2 roles, **Driver** and **Navigator**
    - **Driver**
      - only one whos hands are on the computer
      - handling the mechanics of coding
    - **Navigator**
      - guides the driver
      - thinks big picture

-------------

## Things I want to know more about

- does absolute positioning need the parent element to be set to relative?
- how does box-sizing: border-box; relate to this  
- how memory and variables work, a little deep for me now
