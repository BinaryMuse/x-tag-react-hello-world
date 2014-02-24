This is an experiment with [x-tags](http://www.x-tags.org/) and [react-xtags](https://github.com/vjeux/react-xtags/). This requires changes from [facebook/react#1167](https://github.com/facebook/react/pull/1167); a build from that branch is vendored in `public/js/vendor`.

The idea here is to use x-tags to register new tag types, and to transparently run React components whenever a tag is added to the DOM or is modified; see `public/index.html`.

Running
-------

`npm install && npm start`
