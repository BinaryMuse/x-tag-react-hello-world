This is an experiment with [x-tags](http://www.x-tags.org/) and [react-xtags](https://github.com/vjeux/react-xtags/). This requires changes from [facebook/react#1167](https://github.com/facebook/react/pull/1167); a build from that branch is vendored in `public/js/vendor`.

The idea here is to use x-tags to register new tag types that point to React components.

```javascript
/** @jsx React.DOM */
var Hello = React.createClass({
  render: function() {
    return <div>Hello {this.props.name}!</div>;
  }
});

xreact.register('x-hello', Hello);
```

Adding a node to the DOM or modifying an existing node will transparently render the React component.

```javascript
var hello = document.createElement('x-hello');
hello.setAttribute('name', 'World');
document.querySelector('body').appendChild(hello);
```

Running
-------

`npm install && npm start`
