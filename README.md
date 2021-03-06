# jade loader for webpack

## Usage

``` javascript
var template = require("jade!./file.jade");
// => returns file.jade content as template function
```

[Documentation: Using loaders](http://webpack.github.io/docs/using-loaders.html)

### Embedded resources

Try to use `require` for all your embedded resources, to process them with webpack.

``` jade
div
  img(src=require("./my/image.png"))
```

You need to configure loaders for these filetypes too. (Take a look at the [file-loader](https://github.com/webpack/file-loader).)

## License

MIT (http://www.opensource.org/licenses/mit-license.php)
