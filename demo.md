<script src="https://unpkg.com/babel-standalone@6/babel.min.js"></script>
<script src="https://unpkg.com/react@15.6.1/dist/react.js"></script>
<script src="https://unpkg.com/react-dom@15.6.1/dist/react-dom.js"></script>
<link rel="stylesheet" type="text/css" href="https://unpkg.com/prismjs@1.6.0/themes/prism-tomorrow.css"/>
<style>
body {
  font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Oxygen, Ubuntu, Cantarell, "Open Sans", "Helvetica Neue", sans-serif;
  background: hsl(0, 0%, 90%);
}
pre {
  color: hsl(0, 0%, 90%);
  background: hsl(0, 0%, 10%);
  padding: 10px;
  border-top-right-radius: 6px;
  border-top-left-radius: 6px;
  margin-bottom: 0;
}
.render-js {
  background: white;
  border: 2px solid hsl(0, 0%, 10%);
  padding: 10px;
  border-bottom-right-radius: 6px;
  border-bottom-left-radius: 6px;
}
</style>

# Actually render your code blocks

But this is my markdown file

```render-babel
const h = React.createElement

class Demo extends React.Component {
  componentDidMount() {
    setInterval(() => this.forceUpdate(), 500)
  }
  render() {
    return <h1>This is cool times {Date.now()}</h1>
  }
}

ReactDOM.render(
  <Demo/>,
  DOM_NODE
)
```

Isn't that

- Cool
- Awesome
- Incredibly inflexible?

Yes.