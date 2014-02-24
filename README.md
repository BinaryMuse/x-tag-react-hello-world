This is an experiment with [x-tags](http://www.x-tags.org/) and [react-xtags](https://github.com/vjeux/react-xtags/). Modifications to `react-0.9.0.js` file had to be made; I will open a pull request on the React project to fix these. In the meantime, use the JS from the `public/js/vendor` directory.

The idea here is to use x-tags to register new tag types, and to transparently run React components to render them whenever their properties change. In addition, simple additions to the DOM can be used to render more; see `index.html`.

Running
-------

`npm install && npm start`
