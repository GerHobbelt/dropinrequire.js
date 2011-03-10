# Drop-In require

[dropinrequire.js](http://jeromeetienne.github.com/dropinrequire.js)
is a drop-in replacement for commonjs [module](http://www.commonjs.org/specs/modules/1.0/)
in a browser. No server to run, No preprocessing of javascript files.
If you are using [node.js](http://nodejs.org) and is willing to share code with your browser without
hassle, [dropinrequire.js](http://jeromeetienne.github.com/dropinrequire.js) is for you.

## How to use it

You just include this in your webpage

    <script type="text/javascript" src="./dropin_require.js"></script>

And after that you can use require(filename) to import your node module in the
web browser. 
Suppose you got a module `foobar.js`

    exports.foo	= "bar";

then this html will display `bar`. Here it is a [demo](http://jeromeetienne.github.com/dropinrequire.js/demo/) to show, and not tell.

    <script src="../dropin_require.js"></script>
    <script>
        alert( require('./foobar.js').foo );
    </script>

## About

The code is available on [github](https://github.com/jeromeetienne/dropinrequire.js) under
[MIT license](https://github.com/jeromeetienne/dropinrequire.js/blob/master/MIT-LICENSE.txt) and has been
written by [Jerome Etienne](http://jetienne.com).
That's it. No fuss no muss.

