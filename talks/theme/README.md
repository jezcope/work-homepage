Reveal.js theme for the University Library, University of Sheffield.

## Example of use

```html
<!doctype html>
<html lang="en">
  <head>
    <meta charset="utf-8"/>
    <title>Nice example</title>

    <!-- Include reveal.js styles -->
    <link rel="stylesheet" href="http://cdn.jsdelivr.net/reveal.js/3.0.0/css/reveal.css"/>

    <!-- Include theme -->
    <link rel="stylesheet" href="./css/tuos-lib-blue.css" id="theme"/>
  </head>

  <body>
    <div class="reveal">
      <div class="slides">

        <section>
          <h2>Slide example</h2>

          <p>Put your content here...</p>
        </section>
        
      </div>
    </div>

    <script src="http://cdn.jsdelivr.net/reveal.js/3.0.0/lib/js/head.min.js"></script>
    <script src="http://cdn.jsdelivr.net/reveal.js/3.0.0/js/reveal.js"></script>

    <script>
      Reveal.initialize({});
    </script>
  </body>
</html>
```

## License

All content is copyright © 2017 University of Sheffield and may not be used or reproduced without permission, with the following exceptions:

`templates` directory
: Copyright © 2017 Hakim El Hattab, http://hakim.se, and reveal.js contributors: available under the [MIT License](https://github.com/hakimel/reveal.js/blob/master/LICENSE)
