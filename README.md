# suppress-files-webpack-plugin
Webpack plugin for removing files with names that match a regex from the build output.


<div align="center">
  <!-- replace with accurate logo e.g from https://worldvectorlogo.com/ -->
  <a href="https://github.com/webpack/webpack">
    <img width="200" height="200" vspace="" hspace="25"
      src="https://cdn.rawgit.com/webpack/media/e7485eb2/logo/icon.svg">
  </a>
  <h1>Suppress Files Webpack Plugin</h1>
  <p>Removes files from build output by regex match on file names.<p>
</div>

When working with complex Webpack builds and async loaded chunks, sometimes you need to exclude or suppress certain files from being outputted.

<h2 align="center">Install</h2>

```bash
$ npm install --save-dev suppress-files-webpack-plugin
```

<h2 align="center">Usage</h2>

In your `webpack.config.js`:

```js
plugins: [
  new SuppressFilesPlugin({
    match: /\.js$/
  })
],
```

You can provide a `RegExp` to the `match` parameter which is compared against the file name of the chunk.  Anything that matches will be deleted from the outputted build.

<h2 align="center">Maintainers</h2>

<table>
  <tbody>
    <tr>
      <td align="center">
        <a href="https://github.com/iamdavidjackson">David Jackson</a>
      </td>
    </tr>
  <tbody>
</table>