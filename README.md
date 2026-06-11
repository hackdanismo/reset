# reset

## What is a CSS reset?
A `CSS reset` is a small set of CSS rules that removes the browser's default styling for `HTML` elements and creates a consistent style across all browsers to provide a more predictable starting point.

## How to use
Download the `reset.css` or `reset.min.css` stylesheets and add to your web project in the same location as all other CSS stylesheets. It is recommended to use the `reset.min.css` stylesheet for production as this has a reduced file size and has been optimised for production websites.

+ [reset.css](https://github.com/hackdanismo/reset/blob/main/reset.css)
+ [reset.min.css](https://github.com/hackdanismo/reset/blob/main/reset.min.css)

Once downloaded, add the reset to the `<head>` section of your `HTML`.

```html
<!DOCTYPE html>
<html lang="en">
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>Webpage Title</title>

    <!-- Include the reset CSS stylsheet -->
    <link rel="stylesheet" href="reset.min.css">
</html>
```

The `reset` will now be added to your webpage.

## Development

### Clone the repository
To cloen the repository locally, use the following terminal commands:

```shell
# SSH
$ git clone git@github.com:hackdanismo/reset.git
# HTTPS
$ git clone https://github.com/hackdanismo/reset.git

# Change directory once the repo is cloned
$ cd reset
```

### Set the Node version
It is recommended to set `Node` to the recommended version. For this [nvm](https://github.com/nvm-sh/nvm) `(Node Version Manager)` is used.

```shell
# This will set the recommended Node version, if installed, using nvm
$ nvm use
```

### Minify the stylesheet
CSS changes should be made inside of the `reset.css` stylesheet file. Once changes are made, the minified file, `reset.min.css` should be updated. The `clean-css-cli` npm package is used to minify the CSS code.

```shell
$ npm run minify:css
```

## Licence
The project is created by `Dan Jackson` and relased under the [MIT licence](https://github.com/hackdanismo/reset/blob/main/LICENSE).