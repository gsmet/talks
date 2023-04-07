# How to launch this presentation

1. Install [Node.js](http://nodejs.org/) and [Grunt](http://gruntjs.com/getting-started#installing-the-cli)

   On Fedora:
   ```sh
   $ sudo dnf install npm ; sudo npm install -g grunt-cli
   ```

2. Install dependencies of this project (run within the git checkout):
   ```sh
   $ npm install
   ```

3. Serve the presentation (run within the git checkout):
   ```sh
   $ npm start
   ```

4. Open <http://localhost:8000> to view your presentation.

The presentations can be published to the `gh-pages` branch with the following command:
```sh
$ grunt publish
```

## SVG

SVG sources are in the `sources` directory.
Do not modify the compressed SVG files that are in the `content` directory.

To embed the fonts in a SVG, use [Vecta nano](https://vecta.io/nano).
