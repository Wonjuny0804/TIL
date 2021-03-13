# Today I learned

I have been learning about React these days. So I shall organize the things that I have learned in this repository

So I have learned that React uses JSX syntax which are quite different from normal JavaScript syntax. Basically JSX is a abbreviation for JavaScript Syntax eXtention. Genrally people would use JSX for programming React. 

One might wondere how the JSX goes right? Here's some example codes for them. 
```JSX
<button 
  type="button"
  className="button button__resolve
  ">
  Submit
</button>
```

Things above might seem like a HTML code. However we can see that the class is in "className". So why is this? Because it's actually a JSX. 

How React works is that it the Babel extention inside React will compile JSX code into a React Element. Eventually something that looks like this. 

```JSX
React.createElement(
  'button', 
  {
    type: 'button',
    className: 'button button__resolve'
  },
  'Submit'
)
```

Although a React element isn't a real existing element. It's a JavaScript Object that abstracts a react element. 

So is JSX neccessary? well not really... According to the books and materials I've read and studied. They all say that if you want to code React, you can either use JSX or just plain JavaScript with the method `React.createElement`.

## Some features about React...
At this point React is one of the most famous Frontend Libraries. With React people are able to create Web-apps and mobile native apps. 

If you go to the [React.js official website](www.reactjs.org) then you will see React's most vivid features. 
- Declarative
- Component-Based
- Learn Once, Write Anywhere

and of course on JSConf they said the key to React's algorithm was "Reconcilliation" not Mutation.